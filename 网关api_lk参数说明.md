## 背景

- 网关的请求调用量非常大，每天api的调用量日志达到几十GB，因此，不可能像业务系统那样，把所有请求的入参、出参都打印出来。但是有些业务方又非常"固执"，一定要看到自己的"错误"才肯罢休；因此。网关这边提供了一个扩展属性，专门用来为某些api打印出参日志，方便排查问题。

## 如何使用

### 适用对象

- 参数对象：只能作用于query参数 或 (表单提交并且contentType为**application/x-www-form-urlencode**)的请求参数。
- 参数层级：只能作用于第一层
- api：不是所有的api都适合开启此功能，**核心是不能让参数打印的日志过大，防止服务器的磁盘利用率快速递增**。主要的宗旨是：**流量小的api可以打印全部参数，流量大的api（比如fullinfo）最好只打印部分核心日志，方便排查问题。问题排查结束后，记得关闭扩展参数****。**

### 使用示例

- 以**taobao.logistics.express.delivery.shsm.call.request** api为例，打印入参

#### 第一步：查看api的定义文件

- 查看链接：[**http://api.alibaba-inc.com/system/apidefine?spm=a1zac.8200458.2271772.7.1a136bf7lvdPfT**](http://api.alibaba-inc.com/system/apidefine?spm=a1zac.8200458.2271772.7.1a136bf7lvdPfT)

```xml
<api name="taobao.logistics.express.delivery.shsm.call.request">
    <platform>
        <session>NO_NEED</session>
        <privilege_level>R1</privilege_level>
    </platform>
    <application>
        <params>
            <param name="taobao_logistics_express_delivery_shsm_call_request" requireType="REQUIRED" type="json">
                <param name="request_time" requireType="REQUIRED" type="date"/>
                <param name="supplier_id" requireType="REQUIRED" type="string"/>
                <param name="operator_id" requireType="REQUIRED" type="string"/>
                <param name="cp_code" requireType="REQUIRED" type="string"/>
                <param name="delivery_code" requireType="REQUIRED" type="string"/>
                <param name="delivery_name" requireType="REQUIRED" type="string"/>
                <param max_list_size="999" name="package_infos" requireType="REQUIRED" type="json">
                    <param name="biz_code" requireType="REQUIRED" type="string"/>
                    <param name="mail_no" requireType="REQUIRED" type="string"/></param>
            </param>
        </params>
    </application>
    <service group="HSF" method="sendCall" name="com.alibaba.tt.logistics.cs.infra.client.service.IvrCallClient" timeout="3000" type="hsf" version="1.0.0">
        <request>
            <param apiName="taobao_logistics_express_delivery_shsm_call_request" class="com.alibaba.tt.logistics.cs.infra.client.dto.CallRequest" name="CallRequest" transferType="api" type="struct">
                <param apiName="request_time" class="java.util.Date" name="requestTime" transferType="api"/>
                <param apiName="supplier_id" class="java.lang.String" name="supplierId" transferType="api"/>
                <param apiName="operator_id" class="java.lang.String" name="operatorId" transferType="api"/>
                <param apiName="cp_code" class="java.lang.String" name="cpCode" transferType="api"/>
                <param apiName="delivery_code" class="java.lang.String" name="deliveryCode" transferType="api"/>
                <param apiName="delivery_name" class="java.lang.String" name="deliveryName" transferType="api"/>
                <param apiName="package_infos" class="com.alibaba.tt.logistics.cs.infra.client.dto.PackageInfo" listType="list" name="packageInfos" transferType="api" type="struct">
                    <param apiName="biz_code" class="java.lang.String" name="bizCode" transferType="api"/>
                    <param apiName="mail_no" class="java.lang.String" name="mailNo" transferType="api"/></param>
            </param>
        </request>
        <response>
            <param apiName="taobao_logistics_express_delivery_shsm_call_response" transferType="api" type="struct">
                <param apiName="success" class="java.lang.Boolean" name="success" transferType="api"/>
                <param apiName="error_code" class="java.lang.String" name="errorCode" transferType="api"/>
                <param apiName="error_message" class="java.lang.String" name="errorMsg" transferType="api"/></param>
        </response>
        <error>
            <errorHandler type="exception">
                <errorCode value="isp.taobao_logistics_express_delivery_shsm_call_error"/>
                <errorMessage value="送货上门外呼请求失败"/>
            </errorHandler>
        </error>
    </service>
</api>
```

- 关注application下的params节点![img](https://intranetproxy.alipay.com/skylark/lark/0/2024/png/30356712/1707192556924-9882bcac-c19f-4292-8518-97805e71cd7b.png)

#### 第二步：确定param节点 && 组装扩展属性value

- params节点下面可以有多个param节点，每个param可以是一个json，也可以是一个list对象。

注意：这里的param节点是指![img](https://intranetproxy.alipay.com/skylark/lark/0/2024/png/30356712/1707192664071-1236882a-c43e-41f0-8343-0389b1019426.png)**外层的param节点，而不是param里面的param节点！**

- 确定param节点的类型。

- - 如果是list类别。则组装value为：**list:taobao_logistics_express_delivery_shsm_call_request** 这将表示获取参数类别**为list**，参数名为taobao_logistics_express_delivery_shsm_call_request的参数。
  - 如果是非list类别（上图格式）。则组装value为：**taobao_logistics_express_delivery_shsm_call_request** 这将表示获取参数类别为**非list**，参数名为taobao_logistics_express_delivery_shsm_call_request的参数。

- 以当前示例为例：taobao_logistics_express_delivery_shsm_call_request为非list，因此只需要组装value为：**taobao_logistics_express_delivery_shsm_call_request** 即可

#### 第三步：配置api的扩展属性

- 在此页面查找api：https://topadmin.alibaba-inc.com/api/apiList
- 点击进入api详情：![img](https://intranetproxy.alipay.com/skylark/lark/0/2024/png/30356712/1707193022957-f156d88b-7fcc-4726-a571-d17837f5691f.png)
- 进入扩展属性页面，添加扩展属性即可：![img](https://intranetproxy.alipay.com/skylark/lark/0/2024/png/30356712/1707193143130-98747b5f-666a-4656-bfea-9d0bb0e18374.png)

多个参数名，用英文逗号隔开



## 注意事项

- **参数对象：****只能作用于query参数 或 (表单提交并且contentType为application/x-www-form-urlencode)的请求参数。**
- **参数层级：****只能作用于第一层**
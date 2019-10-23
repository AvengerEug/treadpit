<!-- TOC -->

- [一. 前端](#%e4%b8%80-%e5%89%8d%e7%ab%af)
  - [1.1 Css/Scss](#11-cssscss)
    - [1.1.1 层叠性](#111-%e5%b1%82%e5%8f%a0%e6%80%a7)
    - [1.1.2 继承性](#112-%e7%bb%a7%e6%89%bf%e6%80%a7)
    - [1.1.3 优先级](#113-%e4%bc%98%e5%85%88%e7%ba%a7)
    - [1.1.4 backgroud设置背景图片样式顺序决定是否生效](#114-backgroud%e8%ae%be%e7%bd%ae%e8%83%8c%e6%99%af%e5%9b%be%e7%89%87%e6%a0%b7%e5%bc%8f%e9%a1%ba%e5%ba%8f%e5%86%b3%e5%ae%9a%e6%98%af%e5%90%a6%e7%94%9f%e6%95%88)
    - [1.1.5 Vue在元素中要使用当前vue对象的属性作为图片路径显示在 background-image: url() css上解决办法:](#115-vue%e5%9c%a8%e5%85%83%e7%b4%a0%e4%b8%ad%e8%a6%81%e4%bd%bf%e7%94%a8%e5%bd%93%e5%89%8dvue%e5%af%b9%e8%b1%a1%e7%9a%84%e5%b1%9e%e6%80%a7%e4%bd%9c%e4%b8%ba%e5%9b%be%e7%89%87%e8%b7%af%e5%be%84%e6%98%be%e7%a4%ba%e5%9c%a8-background-image-url-css%e4%b8%8a%e8%a7%a3%e5%86%b3%e5%8a%9e%e6%b3%95)
    - [1.1.6 div里面的内容如何垂直居中](#116-div%e9%87%8c%e9%9d%a2%e7%9a%84%e5%86%85%e5%ae%b9%e5%a6%82%e4%bd%95%e5%9e%82%e7%9b%b4%e5%b1%85%e4%b8%ad)
    - [1.1.7 RGBA](#117-rgba)
    - [1.1.8 块级元素](#118-%e5%9d%97%e7%ba%a7%e5%85%83%e7%b4%a0)
    - [1.1.9 行级元素](#119-%e8%a1%8c%e7%ba%a7%e5%85%83%e7%b4%a0)
    - [1.1.10 行内块元素](#1110-%e8%a1%8c%e5%86%85%e5%9d%97%e5%85%83%e7%b4%a0)
    - [1.1.11 行高](#1111-%e8%a1%8c%e9%ab%98)
    - [1.1.12 浮动](#1112-%e6%b5%ae%e5%8a%a8)
  - [1.2 Java Script](#12-java-script)
    - [1.2.1 Object.assign](#121-objectassign)
    - [1.2.2 前端js获取滚动条距离顶部的位置](#122-%e5%89%8d%e7%ab%afjs%e8%8e%b7%e5%8f%96%e6%bb%9a%e5%8a%a8%e6%9d%a1%e8%b7%9d%e7%a6%bb%e9%a1%b6%e9%83%a8%e7%9a%84%e4%bd%8d%e7%bd%ae)
    - [1.2.3 splice删除指定数组下标](#123-splice%e5%88%a0%e9%99%a4%e6%8c%87%e5%ae%9a%e6%95%b0%e7%bb%84%e4%b8%8b%e6%a0%87)
    - [1.2.4 Object.keys(), Object.values()](#124-objectkeys-objectvalues)
    - [1.2.5 addEventListener注册事件注意点](#125-addeventlistener%e6%b3%a8%e5%86%8c%e4%ba%8b%e4%bb%b6%e6%b3%a8%e6%84%8f%e7%82%b9)
  - [1.3 Vue.js/Nuxt.js](#13-vuejsnuxtjs)
    - [1.3.1 vue.js生命周期](#131-vuejs%e7%94%9f%e5%91%bd%e5%91%a8%e6%9c%9f)
    - [1.3.2 nuxt.js 生命周期](#132-nuxtjs-%e7%94%9f%e5%91%bd%e5%91%a8%e6%9c%9f)
    - [1.3.3 computed(计算属性)](#133-computed%e8%ae%a1%e7%ae%97%e5%b1%9e%e6%80%a7)
    - [1.3.4 v-show和v-if](#134-v-show%e5%92%8cv-if)
    - [1.3.5 v-for](#135-v-for)
    - [1.3.6 this.$set/Vue.set 响应式属性](#136-thissetvueset-%e5%93%8d%e5%ba%94%e5%bc%8f%e5%b1%9e%e6%80%a7)
    - [1.3.7 自定义指令](#137-%e8%87%aa%e5%ae%9a%e4%b9%89%e6%8c%87%e4%bb%a4)
    - [1.3.8 vue-router base属性](#138-vue-router-base%e5%b1%9e%e6%80%a7)
    - [1.3.9 Nuxt v-for嵌套v-if的坑](#139-nuxt-v-for%e5%b5%8c%e5%a5%97v-if%e7%9a%84%e5%9d%91)
    - [1.3.10 .native添加原生事件](#1310-native%e6%b7%bb%e5%8a%a0%e5%8e%9f%e7%94%9f%e4%ba%8b%e4%bb%b6)
    - [1.3.11 nuxt.js重定向](#1311-nuxtjs%e9%87%8d%e5%ae%9a%e5%90%91)
    - [1.3.12 vue深度监听属性](#1312-vue%e6%b7%b1%e5%ba%a6%e7%9b%91%e5%90%ac%e5%b1%9e%e6%80%a7)
    - [1.3.13 vue脚手架3.0版本之前的路由配置](#1313-vue%e8%84%9a%e6%89%8b%e6%9e%b630%e7%89%88%e6%9c%ac%e4%b9%8b%e5%89%8d%e7%9a%84%e8%b7%af%e7%94%b1%e9%85%8d%e7%bd%ae)
    - [1.3.14 前端生成excel表格](#1314-%e5%89%8d%e7%ab%af%e7%94%9f%e6%88%90excel%e8%a1%a8%e6%a0%bc)
    - [1.3.15 限制输入字符的语句在linux中会失效](#1315-%e9%99%90%e5%88%b6%e8%be%93%e5%85%a5%e5%ad%97%e7%ac%a6%e7%9a%84%e8%af%ad%e5%8f%a5%e5%9c%a8linux%e4%b8%ad%e4%bc%9a%e5%a4%b1%e6%95%88)
    - [1.3.15 vue.js嵌套路由 子路由path的定义](#1315-vuejs%e5%b5%8c%e5%a5%97%e8%b7%af%e7%94%b1-%e5%ad%90%e8%b7%af%e7%94%b1path%e7%9a%84%e5%ae%9a%e4%b9%89)
    - [1.3.16 Nuxt.js 官网提供的自定义loading组件. 并将该组件定义在nuxt.config.js的loading 选项中](#1316-nuxtjs-%e5%ae%98%e7%bd%91%e6%8f%90%e4%be%9b%e7%9a%84%e8%87%aa%e5%ae%9a%e4%b9%89loading%e7%bb%84%e4%bb%b6-%e5%b9%b6%e5%b0%86%e8%af%a5%e7%bb%84%e4%bb%b6%e5%ae%9a%e4%b9%89%e5%9c%a8nuxtconfigjs%e7%9a%84loading-%e9%80%89%e9%a1%b9%e4%b8%ad)
    - [1.3.17 vue.js父子组件加载顺序](#1317-vuejs%e7%88%b6%e5%ad%90%e7%bb%84%e4%bb%b6%e5%8a%a0%e8%bd%bd%e9%a1%ba%e5%ba%8f)
    - [1.3.18 vue.js .sync修饰符](#1318-vuejs-sync%e4%bf%ae%e9%a5%b0%e7%ac%a6)
  - [1.4 ElementUI](#14-elementui)
  - [1.5 npm](#15-npm)
    - [1.5.1 package.lock.json](#151-packagelockjson)
    - [1.5.2 package.json文件中的依赖](#152-packagejson%e6%96%87%e4%bb%b6%e4%b8%ad%e7%9a%84%e4%be%9d%e8%b5%96)
    - [1.5.3 npm install指定版本依赖并保存至package.json](#153-npm-install%e6%8c%87%e5%ae%9a%e7%89%88%e6%9c%ac%e4%be%9d%e8%b5%96%e5%b9%b6%e4%bf%9d%e5%ad%98%e8%87%b3packagejson)
    - [1.5.4 npm发布自己编写的vue.js组件库](#154-npm%e5%8f%91%e5%b8%83%e8%87%aa%e5%b7%b1%e7%bc%96%e5%86%99%e7%9a%84vuejs%e7%bb%84%e4%bb%b6%e5%ba%93)
    - [1.5.5 npm+git搭建私有npm仓库](#155-npmgit%e6%90%ad%e5%bb%ba%e7%a7%81%e6%9c%89npm%e4%bb%93%e5%ba%93)
  - [1.6 Html](#16-html)
    - [1.6.1 手动设置ie浏览器以最新版本渲染页面](#161-%e6%89%8b%e5%8a%a8%e8%ae%be%e7%bd%aeie%e6%b5%8f%e8%a7%88%e5%99%a8%e4%bb%a5%e6%9c%80%e6%96%b0%e7%89%88%e6%9c%ac%e6%b8%b2%e6%9f%93%e9%a1%b5%e9%9d%a2)
    - [1.6.2 指定浏览器对html文件的编码格式](#162-%e6%8c%87%e5%ae%9a%e6%b5%8f%e8%a7%88%e5%99%a8%e5%af%b9html%e6%96%87%e4%bb%b6%e7%9a%84%e7%bc%96%e7%a0%81%e6%a0%bc%e5%bc%8f)
  - [1.7 ES6语法](#17-es6%e8%af%ad%e6%b3%95)
    - [1.7.1 export 和 export default的区别](#171-export-%e5%92%8c-export-default%e7%9a%84%e5%8c%ba%e5%88%ab)
- [二. 后端](#%e4%ba%8c-%e5%90%8e%e7%ab%af)
  - [2.1 Java basic](#21-java-basic)
    - [2.1.1 Double引发的Null Pointer Exception](#211-double%e5%bc%95%e5%8f%91%e7%9a%84null-pointer-exception)
    - [2.1.2 强转类型前提](#212-%e5%bc%ba%e8%bd%ac%e7%b1%bb%e5%9e%8b%e5%89%8d%e6%8f%90)
    - [2.1.3 基础数据类型相等的判断](#213-%e5%9f%ba%e7%a1%80%e6%95%b0%e6%8d%ae%e7%b1%bb%e5%9e%8b%e7%9b%b8%e7%ad%89%e7%9a%84%e5%88%a4%e6%96%ad)
    - [2.1.4 Split方法](#214-split%e6%96%b9%e6%b3%95)
    - [2.1.5 异常中try, finally, catch中return的顺序](#215-%e5%bc%82%e5%b8%b8%e4%b8%adtry-finally-catch%e4%b8%adreturn%e7%9a%84%e9%a1%ba%e5%ba%8f)
    - [2.1.6 Servlet中没有暴露出无参构造器(手动编写了带参构造器)](#216-servlet%e4%b8%ad%e6%b2%a1%e6%9c%89%e6%9a%b4%e9%9c%b2%e5%87%ba%e6%97%a0%e5%8f%82%e6%9e%84%e9%80%a0%e5%99%a8%e6%89%8b%e5%8a%a8%e7%bc%96%e5%86%99%e4%ba%86%e5%b8%a6%e5%8f%82%e6%9e%84%e9%80%a0%e5%99%a8)
    - [2.1.7 根据oss url获取远程图片, 并转成base64](#217-%e6%a0%b9%e6%8d%aeoss-url%e8%8e%b7%e5%8f%96%e8%bf%9c%e7%a8%8b%e5%9b%be%e7%89%87-%e5%b9%b6%e8%bd%ac%e6%88%90base64)
    - [2.1.8 动态代理抛出实际真实异常](#218-%e5%8a%a8%e6%80%81%e4%bb%a3%e7%90%86%e6%8a%9b%e5%87%ba%e5%ae%9e%e9%99%85%e7%9c%9f%e5%ae%9e%e5%bc%82%e5%b8%b8)
    - [2.1.9 多线程基础](#219-%e5%a4%9a%e7%ba%bf%e7%a8%8b%e5%9f%ba%e7%a1%80)
      - [2.1.9.1 volatile关键字与System.out.print的欢喜冤家](#2191-volatile%e5%85%b3%e9%94%ae%e5%ad%97%e4%b8%8esystemoutprint%e7%9a%84%e6%ac%a2%e5%96%9c%e5%86%a4%e5%ae%b6)
      - [2.1.9.2 JDK线程状态及转换图](#2192-jdk%e7%ba%bf%e7%a8%8b%e7%8a%b6%e6%80%81%e5%8f%8a%e8%bd%ac%e6%8d%a2%e5%9b%be)
    - [2.1.10 抽象类和接口的区别](#2110-%e6%8a%bd%e8%b1%a1%e7%b1%bb%e5%92%8c%e6%8e%a5%e5%8f%a3%e7%9a%84%e5%8c%ba%e5%88%ab)
    - [2.1.11 Overload和Override的区别](#2111-overload%e5%92%8coverride%e7%9a%84%e5%8c%ba%e5%88%ab)
    - [2.1.12 ArrayList，LinkedList，Vector](#2112-arraylistlinkedlistvector)
    - [2.1.13 HashMap, HashTable, ConcurrentHashMap](#2113-hashmap-hashtable-concurrenthashmap)
    - [2.1.14 创建Class对象的几种方法](#2114-%e5%88%9b%e5%bb%baclass%e5%af%b9%e8%b1%a1%e7%9a%84%e5%87%a0%e7%a7%8d%e6%96%b9%e6%b3%95)
    - [2.1.15 ArrayList.asList()的坑](#2115-arraylistaslist%e7%9a%84%e5%9d%91)
    - [2.1.16 不要在 foreach 循环里进行元素的 remove/add 操作](#2116-%e4%b8%8d%e8%a6%81%e5%9c%a8-foreach-%e5%be%aa%e7%8e%af%e9%87%8c%e8%bf%9b%e8%a1%8c%e5%85%83%e7%b4%a0%e7%9a%84-removeadd-%e6%93%8d%e4%bd%9c)
    - [2.1.17 JVM 类加载器](#2117-jvm-%e7%b1%bb%e5%8a%a0%e8%bd%bd%e5%99%a8)
  - [2.2 Spring Cloud](#22-spring-cloud)
    - [2.2.1 服务注册中心Eureka](#221-%e6%9c%8d%e5%8a%a1%e6%b3%a8%e5%86%8c%e4%b8%ad%e5%bf%83eureka)
    - [2.2.2 ApiGateWay(Zuul)](#222-apigatewayzuul)
    - [2.2.3 FeignClient](#223-feignclient)
    - [2.2.4 Swagger](#224-swagger)
    - [2.2.5 ServerConfig](#225-serverconfig)
    - [2.2.6 SpringCloud常用组件及作用](#226-springcloud%e5%b8%b8%e7%94%a8%e7%bb%84%e4%bb%b6%e5%8f%8a%e4%bd%9c%e7%94%a8)
  - [2.3 Spring Boot](#23-spring-boot)
    - [2.3.1 @RequestParam 类型映射](#231-requestparam-%e7%b1%bb%e5%9e%8b%e6%98%a0%e5%b0%84)
    - [2.3.2 @RequestMapping 方法映射关系](#232-requestmapping-%e6%96%b9%e6%b3%95%e6%98%a0%e5%b0%84%e5%85%b3%e7%b3%bb)
    - [2.3.3 @RequestBody注解接收Post请求ContentType为application/x-www-form-urlencoded格式的数据](#233-requestbody%e6%b3%a8%e8%a7%a3%e6%8e%a5%e6%94%b6post%e8%af%b7%e6%b1%82contenttype%e4%b8%baapplicationx-www-form-urlencoded%e6%a0%bc%e5%bc%8f%e7%9a%84%e6%95%b0%e6%8d%ae)
    - [2.3.4 @RequestMapping支持多种请求方法](#234-requestmapping%e6%94%af%e6%8c%81%e5%a4%9a%e7%a7%8d%e8%af%b7%e6%b1%82%e6%96%b9%e6%b3%95)
    - [2.3.5 @RequestMapping指定request和response的contentType](#235-requestmapping%e6%8c%87%e5%ae%9arequest%e5%92%8cresponse%e7%9a%84contenttype)
    - [2.3.6 SpringBoot使用对象来接收query参数](#236-springboot%e4%bd%bf%e7%94%a8%e5%af%b9%e8%b1%a1%e6%9d%a5%e6%8e%a5%e6%94%b6query%e5%8f%82%e6%95%b0)
    - [2.3.7 Spring mvc 全局异常处理注解@ExceptionHandler](#237-spring-mvc-%e5%85%a8%e5%b1%80%e5%bc%82%e5%b8%b8%e5%a4%84%e7%90%86%e6%b3%a8%e8%a7%a3exceptionhandler)
    - [2.3.8 Spring获取ioc容器上下文的两种方式](#238-spring%e8%8e%b7%e5%8f%96ioc%e5%ae%b9%e5%99%a8%e4%b8%8a%e4%b8%8b%e6%96%87%e7%9a%84%e4%b8%a4%e7%a7%8d%e6%96%b9%e5%bc%8f)
    - [2.3.9 Spring核心](#239-spring%e6%a0%b8%e5%bf%83)
    - [2.3.10 Spring bean生命周期](#2310-spring-bean%e7%94%9f%e5%91%bd%e5%91%a8%e6%9c%9f)
    - [2.3.11 SpringBoot是job注解和异步调用注解生效前提](#2311-springboot%e6%98%afjob%e6%b3%a8%e8%a7%a3%e5%92%8c%e5%bc%82%e6%ad%a5%e8%b0%83%e7%94%a8%e6%b3%a8%e8%a7%a3%e7%94%9f%e6%95%88%e5%89%8d%e6%8f%90)
    - [2.3.12 Springboot yml文件配置的坑](#2312-springboot-yml%e6%96%87%e4%bb%b6%e9%85%8d%e7%bd%ae%e7%9a%84%e5%9d%91)
    - [2.3.13 @Autowired和@Resource的区别](#2313-autowired%e5%92%8cresource%e7%9a%84%e5%8c%ba%e5%88%ab)
    - [2.3.14 SpringBoot默认包扫描路径](#2314-springboot%e9%bb%98%e8%ae%a4%e5%8c%85%e6%89%ab%e6%8f%8f%e8%b7%af%e5%be%84)
  - [2.4 Mybatis](#24-mybatis)
    - [2.4.1 parameterType为int/long时, 参数为0的处理](#241-parametertype%e4%b8%baintlong%e6%97%b6-%e5%8f%82%e6%95%b0%e4%b8%ba0%e7%9a%84%e5%a4%84%e7%90%86)
    - [2.4.2 $和#区别](#242-%e5%92%8c%e5%8c%ba%e5%88%ab)
    - [2.4.3 ORM映射文件 type和map后缀的区别](#243-orm%e6%98%a0%e5%b0%84%e6%96%87%e4%bb%b6-type%e5%92%8cmap%e5%90%8e%e7%bc%80%e7%9a%84%e5%8c%ba%e5%88%ab)
    - [2.4.4 Mybatis resultMap中type=map, 使用枚举的typeHandler前提](#244-mybatis-resultmap%e4%b8%adtypemap-%e4%bd%bf%e7%94%a8%e6%9e%9a%e4%b8%be%e7%9a%84typehandler%e5%89%8d%e6%8f%90)
    - [2.4.5 使用springboot 通过继承SqlSessionDaoSupport类集成mybatis](#245-%e4%bd%bf%e7%94%a8springboot-%e9%80%9a%e8%bf%87%e7%bb%a7%e6%89%bfsqlsessiondaosupport%e7%b1%bb%e9%9b%86%e6%88%90mybatis)
  - [2.5 MySql](#25-mysql)
    - [2.5.1 export database/table command](#251-export-databasetable-command)
    - [2.5.2 import database/table command](#252-import-databasetable-command)
    - [2.5.3 mysql压缩版本()启动步骤](#253-mysql%e5%8e%8b%e7%bc%a9%e7%89%88%e6%9c%ac%e5%90%af%e5%8a%a8%e6%ad%a5%e9%aa%a4)
    - [2.5.5 存储过程](#255-%e5%ad%98%e5%82%a8%e8%bf%87%e7%a8%8b)
    - [2.5.6 DML和DDL概念](#256-dml%e5%92%8cddl%e6%a6%82%e5%bf%b5)
    - [2.5.7 mysql连接数不够](#257-mysql%e8%bf%9e%e6%8e%a5%e6%95%b0%e4%b8%8d%e5%a4%9f)
    - [2.5.8 flyway](#258-flyway)
    - [2.5.9 mysql sql优化](#259-mysql-sql%e4%bc%98%e5%8c%96)
  - [2.6 Elasticsearch](#26-elasticsearch)
    - [2.6.1 linux构建es的坑](#261-linux%e6%9e%84%e5%bb%baes%e7%9a%84%e5%9d%91)
  - [2.7 Redis](#27-redis)
    - [2.7.1 手动暂时性的设置密码](#271-%e6%89%8b%e5%8a%a8%e6%9a%82%e6%97%b6%e6%80%a7%e7%9a%84%e8%ae%be%e7%bd%ae%e5%af%86%e7%a0%81)
    - [2.7.2 redis配置远程支持连接](#272-redis%e9%85%8d%e7%bd%ae%e8%bf%9c%e7%a8%8b%e6%94%af%e6%8c%81%e8%bf%9e%e6%8e%a5)
  - [2.8 Maven](#28-maven)
    - [2.8.1 install maven仓库找不到的jar包](#281-install-maven%e4%bb%93%e5%ba%93%e6%89%be%e4%b8%8d%e5%88%b0%e7%9a%84jar%e5%8c%85)
    - [2.8.2 maven profiles集成springboot build多环境](#282-maven-profiles%e9%9b%86%e6%88%90springboot-build%e5%a4%9a%e7%8e%af%e5%a2%83)
    - [2.8.3 maven pom文件scope解析](#283-maven-pom%e6%96%87%e4%bb%b6scope%e8%a7%a3%e6%9e%90)
    - [2.8.4 maven项目打包类型](#284-maven%e9%a1%b9%e7%9b%ae%e6%89%93%e5%8c%85%e7%b1%bb%e5%9e%8b)
    - [2.8.5 maven代码混淆插件导致spring 创建的bean找不到类型](#285-maven%e4%bb%a3%e7%a0%81%e6%b7%b7%e6%b7%86%e6%8f%92%e4%bb%b6%e5%af%bc%e8%87%b4spring-%e5%88%9b%e5%bb%ba%e7%9a%84bean%e6%89%be%e4%b8%8d%e5%88%b0%e7%b1%bb%e5%9e%8b)
  - [2.9 Git](#29-git)
    - [2.9.1 回退版本](#291-%e5%9b%9e%e9%80%80%e7%89%88%e6%9c%ac)
    - [2.9.2 查看分支树](#292-%e6%9f%a5%e7%9c%8b%e5%88%86%e6%94%af%e6%a0%91)
    - [2.9.3 只查看commitId和comments的背景](#293-%e5%8f%aa%e6%9f%a5%e7%9c%8bcommitid%e5%92%8ccomments%e7%9a%84%e8%83%8c%e6%99%af)
    - [2.9.4 cherry-pick和merge的区别](#294-cherry-pick%e5%92%8cmerge%e7%9a%84%e5%8c%ba%e5%88%ab)
    - [2.9.5 合并commit](#295-%e5%90%88%e5%b9%b6commit)
    - [2.9.6 git reset HEAD~ 带来的坑](#296-git-reset-head-%e5%b8%a6%e6%9d%a5%e7%9a%84%e5%9d%91)
    - [2.9.7 Github中提交的记录在Contribution中看不到](#297-github%e4%b8%ad%e6%8f%90%e4%ba%a4%e7%9a%84%e8%ae%b0%e5%bd%95%e5%9c%a8contribution%e4%b8%ad%e7%9c%8b%e4%b8%8d%e5%88%b0)
  - [2.10 设计模式与应用](#210-%e8%ae%be%e8%ae%a1%e6%a8%a1%e5%bc%8f%e4%b8%8e%e5%ba%94%e7%94%a8)
    - [2.10.1 简单工厂 + java多态性完成订单流水操作](#2101-%e7%ae%80%e5%8d%95%e5%b7%a5%e5%8e%82--java%e5%a4%9a%e6%80%81%e6%80%a7%e5%ae%8c%e6%88%90%e8%ae%a2%e5%8d%95%e6%b5%81%e6%b0%b4%e6%93%8d%e4%bd%9c)
    - [2.10.2 适配器模式 + 动态代理集成第三方类库, 完成日志记录操作](#2102-%e9%80%82%e9%85%8d%e5%99%a8%e6%a8%a1%e5%bc%8f--%e5%8a%a8%e6%80%81%e4%bb%a3%e7%90%86%e9%9b%86%e6%88%90%e7%ac%ac%e4%b8%89%e6%96%b9%e7%b1%bb%e5%ba%93-%e5%ae%8c%e6%88%90%e6%97%a5%e5%bf%97%e8%ae%b0%e5%bd%95%e6%93%8d%e4%bd%9c)
    - [2.10.3 模板方法](#2103-%e6%a8%a1%e6%9d%bf%e6%96%b9%e6%b3%95)
    - [2.10.4 观察者模式](#2104-%e8%a7%82%e5%af%9f%e8%80%85%e6%a8%a1%e5%bc%8f)
- [三. DevOps](#%e4%b8%89-devops)
  - [3.1 Docker](#31-docker)
    - [3.1.1 搭建远程本地仓库](#311-%e6%90%ad%e5%bb%ba%e8%bf%9c%e7%a8%8b%e6%9c%ac%e5%9c%b0%e4%bb%93%e5%ba%93)
    - [3.1.2 push镜像到本地仓库](#312-push%e9%95%9c%e5%83%8f%e5%88%b0%e6%9c%ac%e5%9c%b0%e4%bb%93%e5%ba%93)
    - [3.1.3 使用ssh远程执行命令运行容器](#313-%e4%bd%bf%e7%94%a8ssh%e8%bf%9c%e7%a8%8b%e6%89%a7%e8%a1%8c%e5%91%bd%e4%bb%a4%e8%bf%90%e8%a1%8c%e5%ae%b9%e5%99%a8)
    - [3.1.4 挂载宿主机目录](#314-%e6%8c%82%e8%bd%bd%e5%ae%bf%e4%b8%bb%e6%9c%ba%e7%9b%ae%e5%bd%95)
    - [3.1.5 ADD命令的坑](#315-add%e5%91%bd%e4%bb%a4%e7%9a%84%e5%9d%91)
    - [3.1.6 Dockerfile常见命令解析](#316-dockerfile%e5%b8%b8%e8%a7%81%e5%91%bd%e4%bb%a4%e8%a7%a3%e6%9e%90)
    - [3.1.7 指定docker 容器的时间参照物](#317-%e6%8c%87%e5%ae%9adocker-%e5%ae%b9%e5%99%a8%e7%9a%84%e6%97%b6%e9%97%b4%e5%8f%82%e7%85%a7%e7%89%a9)
  - [3.2 Jenkins](#32-jenkins)
    - [3.2.1 自动化部署maven项目](#321-%e8%87%aa%e5%8a%a8%e5%8c%96%e9%83%a8%e7%bd%b2maven%e9%a1%b9%e7%9b%ae)
    - [3.2.2 多job部署, job间传值](#322-%e5%a4%9ajob%e9%83%a8%e7%bd%b2-job%e9%97%b4%e4%bc%a0%e5%80%bc)
    - [3.2.3 linux不同用户运行jenkins.war](#323-linux%e4%b8%8d%e5%90%8c%e7%94%a8%e6%88%b7%e8%bf%90%e8%a1%8cjenkinswar)
    - [3.2.4 Jenkins支持maven多模块项目(每个模块都是一个git仓库)多环境同时部署思想](#324-jenkins%e6%94%af%e6%8c%81maven%e5%a4%9a%e6%a8%a1%e5%9d%97%e9%a1%b9%e7%9b%ae%e6%af%8f%e4%b8%aa%e6%a8%a1%e5%9d%97%e9%83%bd%e6%98%af%e4%b8%80%e4%b8%aagit%e4%bb%93%e5%ba%93%e5%a4%9a%e7%8e%af%e5%a2%83%e5%90%8c%e6%97%b6%e9%83%a8%e7%bd%b2%e6%80%9d%e6%83%b3)
    - [3.2.5 jenkins multijob build多模块(每个模块都是一个git仓库)](#325-jenkins-multijob-build%e5%a4%9a%e6%a8%a1%e5%9d%97%e6%af%8f%e4%b8%aa%e6%a8%a1%e5%9d%97%e9%83%bd%e6%98%af%e4%b8%80%e4%b8%aagit%e4%bb%93%e5%ba%93)
    - [3.2.6 jenkins Multijob 参数传递规则:](#326-jenkins-multijob-%e5%8f%82%e6%95%b0%e4%bc%a0%e9%80%92%e8%a7%84%e5%88%99)
    - [3.2.7 jenkins使用nohup后台运行jar包](#327-jenkins%e4%bd%bf%e7%94%a8nohup%e5%90%8e%e5%8f%b0%e8%bf%90%e8%a1%8cjar%e5%8c%85)
    - [3.2.8 jenkins运行mvn命令找不到](#328-jenkins%e8%bf%90%e8%a1%8cmvn%e5%91%bd%e4%bb%a4%e6%89%be%e4%b8%8d%e5%88%b0)
  - [3.3 Shell脚本](#33-shell%e8%84%9a%e6%9c%ac)
    - [3.3.1 自定义shell脚本, 完成maven多项目自动拉取远程仓库代码操作](#331-%e8%87%aa%e5%ae%9a%e4%b9%89shell%e8%84%9a%e6%9c%ac-%e5%ae%8c%e6%88%90maven%e5%a4%9a%e9%a1%b9%e7%9b%ae%e8%87%aa%e5%8a%a8%e6%8b%89%e5%8f%96%e8%bf%9c%e7%a8%8b%e4%bb%93%e5%ba%93%e4%bb%a3%e7%a0%81%e6%93%8d%e4%bd%9c)
    - [3.3.2 ENV=${ENV:-"local"} 代码含义](#332-envenv-%22local%22-%e4%bb%a3%e7%a0%81%e5%90%ab%e4%b9%89)
    - [3.3.3 ssh执行远程命令awk命令无法执行的问题](#333-ssh%e6%89%a7%e8%a1%8c%e8%bf%9c%e7%a8%8b%e5%91%bd%e4%bb%a4awk%e5%91%bd%e4%bb%a4%e6%97%a0%e6%b3%95%e6%89%a7%e8%a1%8c%e7%9a%84%e9%97%ae%e9%a2%98)
    - [3.3.4 Sed命令根据key修改文件内容](#334-sed%e5%91%bd%e4%bb%a4%e6%a0%b9%e6%8d%aekey%e4%bf%ae%e6%94%b9%e6%96%87%e4%bb%b6%e5%86%85%e5%ae%b9)
    - [3.3.4 Sed和Rename命令修改文件名](#334-sed%e5%92%8crename%e5%91%bd%e4%bb%a4%e4%bf%ae%e6%94%b9%e6%96%87%e4%bb%b6%e5%90%8d)
  - [3.4 Nginx](#34-nginx)
    - [3.4.1 配置反向代理](#341-%e9%85%8d%e7%bd%ae%e5%8f%8d%e5%90%91%e4%bb%a3%e7%90%86)
    - [3.4.2 配置多个vue.js单页面项目](#342-%e9%85%8d%e7%bd%ae%e5%a4%9a%e4%b8%aavuejs%e5%8d%95%e9%a1%b5%e9%9d%a2%e9%a1%b9%e7%9b%ae)
    - [3.4.3 docker化basic auth(可配)](#343-docker%e5%8c%96basic-auth%e5%8f%af%e9%85%8d)
    - [3.4.4 配置Https证书, 支持https访问.](#344-%e9%85%8d%e7%bd%aehttps%e8%af%81%e4%b9%a6-%e6%94%af%e6%8c%81https%e8%ae%bf%e9%97%ae)
- [四. Linux](#%e5%9b%9b-linux)
  - [4.1 常用命令(常忘)](#41-%e5%b8%b8%e7%94%a8%e5%91%bd%e4%bb%a4%e5%b8%b8%e5%bf%98)
    - [4.1.1 给文件添加可执行权限](#411-%e7%bb%99%e6%96%87%e4%bb%b6%e6%b7%bb%e5%8a%a0%e5%8f%af%e6%89%a7%e8%a1%8c%e6%9d%83%e9%99%90)
    - [4.1.2 删除当前文件夹内所有内容](#412-%e5%88%a0%e9%99%a4%e5%bd%93%e5%89%8d%e6%96%87%e4%bb%b6%e5%a4%b9%e5%86%85%e6%89%80%e6%9c%89%e5%86%85%e5%ae%b9)
    - [4.1.3 压缩当前文件夹为zip包](#413-%e5%8e%8b%e7%bc%a9%e5%bd%93%e5%89%8d%e6%96%87%e4%bb%b6%e5%a4%b9%e4%b8%bazip%e5%8c%85)
    - [4.1.4 解压缩zip压缩包到当前目录](#414-%e8%a7%a3%e5%8e%8b%e7%bc%a9zip%e5%8e%8b%e7%bc%a9%e5%8c%85%e5%88%b0%e5%bd%93%e5%89%8d%e7%9b%ae%e5%bd%95)
    - [4.1.5 查看某个文件的大小](#415-%e6%9f%a5%e7%9c%8b%e6%9f%90%e4%b8%aa%e6%96%87%e4%bb%b6%e7%9a%84%e5%a4%a7%e5%b0%8f)
    - [4.1.6 列出文件夹下面第一级每个文件的大小(包括文件夹和文件)](#416-%e5%88%97%e5%87%ba%e6%96%87%e4%bb%b6%e5%a4%b9%e4%b8%8b%e9%9d%a2%e7%ac%ac%e4%b8%80%e7%ba%a7%e6%af%8f%e4%b8%aa%e6%96%87%e4%bb%b6%e7%9a%84%e5%a4%a7%e5%b0%8f%e5%8c%85%e6%8b%ac%e6%96%87%e4%bb%b6%e5%a4%b9%e5%92%8c%e6%96%87%e4%bb%b6)
    - [4.1.7 查找文件命令](#417-%e6%9f%a5%e6%89%be%e6%96%87%e4%bb%b6%e5%91%bd%e4%bb%a4)
    - [4.1.8 查找某个端口被占用](#418-%e6%9f%a5%e6%89%be%e6%9f%90%e4%b8%aa%e7%ab%af%e5%8f%a3%e8%a2%ab%e5%8d%a0%e7%94%a8)
    - [4.1.9 查看linux各进程内存使用情况](#419-%e6%9f%a5%e7%9c%8blinux%e5%90%84%e8%bf%9b%e7%a8%8b%e5%86%85%e5%ad%98%e4%bd%bf%e7%94%a8%e6%83%85%e5%86%b5)
    - [4.1.10 Linux 启动项目后台保留策略](#4110-linux-%e5%90%af%e5%8a%a8%e9%a1%b9%e7%9b%ae%e5%90%8e%e5%8f%b0%e4%bf%9d%e7%95%99%e7%ad%96%e7%95%a5)
    - [4.1.11 cp -r 命令的坑](#4111-cp--r-%e5%91%bd%e4%bb%a4%e7%9a%84%e5%9d%91)
    - [4.1.12 清除所有log文件(内存不够时)](#4112-%e6%b8%85%e9%99%a4%e6%89%80%e6%9c%89log%e6%96%87%e4%bb%b6%e5%86%85%e5%ad%98%e4%b8%8d%e5%a4%9f%e6%97%b6)
    - [4.1.13 压缩成tar.gz压缩包](#4113-%e5%8e%8b%e7%bc%a9%e6%88%90targz%e5%8e%8b%e7%bc%a9%e5%8c%85)
    - [4.1.14 解压缩tar.gz包](#4114-%e8%a7%a3%e5%8e%8b%e7%bc%a9targz%e5%8c%85)
    - [4.1.15 Linux文件权限查看及无权限解决方案](#4115-linux%e6%96%87%e4%bb%b6%e6%9d%83%e9%99%90%e6%9f%a5%e7%9c%8b%e5%8f%8a%e6%97%a0%e6%9d%83%e9%99%90%e8%a7%a3%e5%86%b3%e6%96%b9%e6%a1%88)
- [五. Http](#%e4%ba%94-http)
  - [5.1 ContentType](#51-contenttype)
- [六. IDEA](#%e5%85%ad-idea)
  - [6.1 快捷键](#61-%e5%bf%ab%e6%8d%b7%e9%94%ae)
    - [6.1.1 查看接口或接口中的方法实现类](#611-%e6%9f%a5%e7%9c%8b%e6%8e%a5%e5%8f%a3%e6%88%96%e6%8e%a5%e5%8f%a3%e4%b8%ad%e7%9a%84%e6%96%b9%e6%b3%95%e5%ae%9e%e7%8e%b0%e7%b1%bb)
- [七. 阿里云oss](#%e4%b8%83-%e9%98%bf%e9%87%8c%e4%ba%91oss)
  - [7.1 上传图片](#71-%e4%b8%8a%e4%bc%a0%e5%9b%be%e7%89%87)
    - [7.1.1 私密上传base64格式图片](#711-%e7%a7%81%e5%af%86%e4%b8%8a%e4%bc%a0base64%e6%a0%bc%e5%bc%8f%e5%9b%be%e7%89%87)
  - [7.2 下载图片](#72-%e4%b8%8b%e8%bd%bd%e5%9b%be%e7%89%87)
    - [7.2.1 前端访问私密图片](#721-%e5%89%8d%e7%ab%af%e8%ae%bf%e9%97%ae%e7%a7%81%e5%af%86%e5%9b%be%e7%89%87)

<!-- /TOC -->

## 一. 前端
### 1.1 Css/Scss
#### 1.1.1 层叠性
```
  浏览器的渲染机制是从上至下, 当有多个样式同时应用到同一个dom元素时, 默认使用最后一个样式。(不考虑手动设置权重的case)
```
#### 1.1.2 继承性
```
  1. 前提: 标签之间是嵌套关系
  2. 文字颜色、字体大小、字体、行高、文字有关的属性都可被继承
  3. 特殊点:
    a标签不能实现字体颜色的集成, 字体大小可被继承
    h1标签不可以继承字体大小, 继承过来会做一些 `计算`.
```
#### 1.1.3 优先级
| 类别     | !important | 行内样式 | id选择器 | 类选择器 | 标签选择器 | 默认样式
| ----| ------ | ------ | ------ | ------ | ------ | ------ |
| 对应权重 |   1000以上  |  1000   |   100   |    10   |     1      | 0
```
  对于所有的选择器, 都会统计权重, 哪个权重大, 使用哪个(若权重一样, 则应用最后一个)
```
#### 1.1.4 backgroud设置背景图片样式顺序决定是否生效
1. backgroud: url('xxxx'); 的样式必须写在最前面。
   eg: background-size: 100%; 的参数才会生效, 因为它是override机制。
   同时可以在background: url('xxx') 接属性。
   eg:  background: url('xxx') no-repeat 100% 100%;  即一次性设置完。
2. 使用background-image: url('xxx') 的方式, 这样则不需要考虑前后顺序
#### 1.1.5 Vue在元素中要使用当前vue对象的属性作为图片路径显示在 background-image: url() css上解决办法:
* 需要使用backgroundImage属性:
```js
  <div class="supply-index" :style="{backgroundImage: 'url(' + attributeObj.image + ')'}"></div>
```
注意: ```使用的是backgroundImage, 而不是background-image```

#### 1.1.6 div里面的内容如何垂直居中
```css
width: 100%;
top: 50%;
transform: translateY(-50%);
```
* 其实top: 50%, 已经是将该dom元素垂直居中了, 但是因为要内容居中, 所以需要Y轴移动元素内容高度的50%, 即transform: translateY(-50%)

#### 1.1.7 RGBA
* RGBA来标识颜色, 第四个参数可以增加透明度

#### 1.1.8 块级元素
* 常用块级元素: div, h1-h6, p, ul, li
* 特点:
    1. 独占一行
    2. 可以设置宽高
    3. 嵌套情况下, 子元素的宽度默认与父类一致
#### 1.1.9 行级元素
* 常用行级元素: span, a, strong, em, del, ins
* 特点:
    1. 在一行上显示
    2. 不能直接设置宽和高(若实在想设置宽和高, 可以设置成行内块元素)
    3. 元素的宽和高就是内容撑开宽和高
#### 1.1.10 行内块元素
* 常用行级元素: input, img
* 特点:
    1. 在一行上显示
    2. 可以设置宽高
#### 1.1.11 行高
* 定义: 浏览器默认文本大小为16px, 行高是基于基线与基线之间的距离 = 文字高度 + 上下边距(padding)
#### 1.1.12 浮动
* 定义: 标准文档流: 自上而下, 自左向右, 块元素独占一行, 行元素在一行上显示, 碰到父边框后换行

### 1.2 Java Script
#### 1.2.1 Object.assign
* 使用方式: 
* 注意事项: 若两个对象的key一致, 那么会覆盖value, key不会重复

#### 1.2.2 前端js获取滚动条距离顶部的位置
``` js
let scrollTop = document.documentElement.scrollTop || document.body.scrollTop
//获取当前window窗体的高度: document.documentElement.clientHeight
window.addEventListener('scroll', function(){}, true) //注册滚动条滚动事件

document.documentElment //获取的是html元素
```

#### 1.2.3 splice删除指定数组下标
```js
arr.splice(0, 1) // => 表示从下标为0开始删除一个元素,
arr.splice(0, 1, 'test') // => 则对arr数组下标为0开始添加一个test元素
```

#### 1.2.4 Object.keys(), Object.values()
* 处理数组的结果, 前者会返回数组的每一个元素对应的下标, 后者会返回每一个元素的value

#### 1.2.5 addEventListener注册事件注意点
1. 首先addEventListener添加的事件是不会被覆盖的
     其次若有层级关系(会冒泡), 则遵循以下规则：
       true的执行顺序在false之前
       true和true之间: 外层的先触发 
       false和false之间: 内层的先触发

### 1.3 Vue.js/Nuxt.js
#### 1.3.1 vue.js生命周期
![vue生命周期](https://github.com/EugeneHuang9638/treadpit/blob/master/vue-life-time.png)
![myself](https://github.com/EugeneHuang9638/treadpit/blob/master/vue-life-myself.jpg)

#### 1.3.2 nuxt.js 生命周期
![nuxt.js生命周期](https://github.com/EugeneHuang9638/treadpit/blob/master/nuxt-life-time.png)
#### 1.3.3 computed(计算属性)
```javascript
/* 举个栗子: 当前vue对象中有一个属性叫imageUrl, 但是因为它只是一个url,在动静分离的项目中,  
如果要显示它必须还要在它前面添加oss host和ip, 所以此时可以使用计算属性对该属性进行处理, 计  
算属性的作用比监听器更好, 因为它自带内存机制. 若this.imageUrl值没有变, 则每次获取计算属性  
时都是从内存中获取
*/
computed: {
  realImageUrl: function() {
    return 'oss host : port ' + this.imageUrl
  }
}
```
* 在vue中computed的属性可以使用箭头函数, 第一个参数为vm(当前vue对象). eg:
```javascript
computed: {
  realImageUrl: vm => {
    return 'oss host : port ' + this.imageUrl
  }
}
```
* 在nuxt中, computed的属性请使用普通函数, 如上述第一种. 若使用箭头函数的方式, 会不定时(有时能将当前vue对象依赖注入到vm参数,
  有时却不能)的出现 ```imageUrl of undefined``` 的错误

#### 1.3.4 v-show和v-if
```css
1. 首先要了解css中display: none; 该属性是将dom元素给隐藏且不占用文档流,但元素依然在网  
   页源码中可见(F12).  
2. v-show指令的功能就是上述所说. 
3. v-if指令的功能是将整个dom处于 '渲染-销毁' 这样的生命周期中. 
4. 区别:  
   v-show: 不管初始值为false/true, 都会先渲染对应的dom元素。 对于需频繁控制dom元素的隐藏/显示的需求, 消耗性能较小.  
   v-if:  懒加载dom元素, 只有当value为true的时候才会对dom元素进行渲染, 若由true -> false, 则会对dom元素的所有  
          属性(绑定的事件, 响应式数据的绑定等)进行销毁. 当由false -> true, 则会重新绑定, 所以相比v-show而言,  
          性能消耗较大.
```

#### 1.3.5 v-for
*  先看以下示例(刚接触vue的学者渲染列表数据的经典写法)
```html
<div v-for="(item, index) of items" :key="index">
  <span>{{item.xxx}}</span>
</div>
```
    强烈建议不要使用上述的写法, 若你是做h5项目下拉式的分页功能倒无大碍. 若你是做web pc使用异步请求动态分页渲染列表  
    时, 它会让你见到```非常奇怪```的数据. 你会发现后面的几页数据(不刷新页面的前提下)始终会与前面一页的数据, 但重新  
    刷新页面时, 数据又正常了。 
    
    出现这样的case主要是因为vue为了减少性能消耗添加缓存的原因. 在vue中, 你可以为每一个dom元素绑定key属性, 改属性  
    是vue使用缓存的依据. 对于上面的例子, 当在web pc使用异步请求动态分页渲染列表的情景下, 若我们使用index作为当前  
    dom元素的key, 那么在渲染后面的页数时, 后面的index基本与上一页准备销毁的dom元素的key一致, vue为了尽可能高效  
    的渲染元素, 若发现销毁队列中的dom元素中与将要渲染的dom元素的key一致, 则会采用销毁掉列中的dom元素进行渲染.

    所以, 在web pc使用异步请求动态分页渲染列表的情景下, 我们应该使用唯一标识作为dom元素的key, 这个唯一标识可以是  
    数据结构中的唯一值或者手动引入第三方uuid类库, 将uuid与dom元素的key绑定.

#### 1.3.6 this.$set/Vue.set 响应式属性
* 众所周知, vue的响应式数据是绑定在data方法中. 举个栗子:
```js
<template>
  <h1>the man's name is: {{man.name}}</h1>
  <h2 v-if="man.age">the man's age is: {{man.age}}</h2>
  <button @click="modifyAge">modify age</button>
</template>

export default {
  data () {
    return {
      man: {
        name: 'eugene'
      }
    }
  },
  methods: {
    modifyAge () {
      this.man.age = 13
    }
  },
  mounted () {
    this.man.age = 12
  }
}

/*
1. 首先, 页面上不会显示 the man's age is 12。 因为age这个属性并不是响应式属性,
2. 其次, 就算点击 modify age button 页面也不会显示 the man's age is 13。 因
   为this.$set/Vue.set方法动态添加响应式属性的前提是对象中的key不存在(在该栗子下,
   虚拟dom树挂载到页面上时, mounted钩子方法就被调用了.), 否则该方法只做更新key对
   应的value操作
3. 要在页面中显示the man's age is 12, 需要两个前提
   A. man对象中无age属性
   B. 在A的前提下调用this.$set(this.main, 'age', 12) 或 Vue.set(this.main, 'a
      ge', 12)方法
*/
```

* 场景: 在当前的vue实例中有一个名为currentUser的对象, 该对象只有一个id的属性, 现需要
  给该对象添加一个name和age属性, 以至于在页面中能够支持响应式渲染。
```js
   方法1: 在初始化vue对象的时候给currentUser对象添加name和age属性 value均为空字符串
   方法2: 使用Vue.set(this.currentUser, 'name', value) or this.$set(this.currentUser, 'name', value)
   方法3: this.currentUser = Object.assign({},  this.currentUser, {
            name: 'Eugene',
            age: 23
          })
          //一定要将Object.assign创建一个新对象并重新赋值给this.currentUser对象, 而不要这样使用
          Object.assign(this.currentUser. {
            name: 'Eugene',
            age: 23
          })
          // 因为Object.assign是将结果作为返回值返回
```

#### 1.3.7 自定义指令
1. 注册全局自定义指令
    ```js
    Vue.directive('disabled', {
      bind: (el, binding) => {
        // bind钩子函数, vue挂载dom元素时会触发, 且只调用一次
      },
      update: (el, binding) => {
        // 虚拟dom树更新时, 该钩子函数会被调用
      }
    }
    ```
    ```最好别在bind钩子函数中操作其他dom元素, 因为它在虚拟dom树被创建时会被触发, 此时html的dom树还没有生成, 无法获取其他dom元素, 至于update钩子函数是否可以获取其他dom元素待确认```

2. 解析
![自定义指令解析](https://github.com/EugeneHuang9638/treadpit/blob/master/understand-directive.jpg)

3. [自定义指令官方文档api](https://cn.vuejs.org/v2/guide/custom-directive.html)

#### 1.3.8 vue-router base属性
```
  添加该属性后 route会默认在每次跳转路由前把这个前缀给加上, 此时在浏览器中添加这个前缀或者不添加这个前缀都能match上路由
```
#### 1.3.9 Nuxt v-for嵌套v-if的坑
如下case:(若v-if 里面包含的标签中要使用的判断是否渲染dom元素的变量, eg如下的{{message.type}}要用到v-if的message, )
```js
    <div v-if="message">{{message.type}}</message>
    一定要将前面的v-if改成v-show, 否则页面会在挂载(mounted钩子函数不会被执行)的时候失败。
    具体错误如下: [nuxt] Error while initializing app DOMException: Failed to execute 'appendChild' on 'Node': This node type does not support this method.
    (前提: message 在实例化vue 对象时 要为false)
```
#### 1.3.10 .native添加原生事件
* 使用组件ui库, 若第三方ui库提供的组件中存在@click事件, 则直接使用@click会生效, 否者请加上.native    
  即 @click.native 表示使用原生的click事件

#### 1.3.11 nuxt.js重定向
```
Nuxt.js 在asyncData方法中使用context上下文的redirect重定向时, 
该方法有三个参数(statusCode, url, params)若只填一个url 则statusCode默认为302
若要传参数(只支持params的参数, 即锚点参数, 若存在query参数的话 重定向会失败), params参数是一个对象, key, value的格式
```
#### 1.3.12 vue深度监听属性
```js
watch: {
  属性: {
    //self: this,
    handler: function(newValue, oldValue) {
      console.log(newValue)
    },
    deep: true
  }
}
```
* 通常在pc端写table组件时会用到, 一般prop为数组时, 这个会常用。
* 使用该方式对数组进行深度监听, 否则普通的监听数组内部数据进行改变时, 不会触发监听事件.
注: 在深度监听方式中, 如果要在里面处理当前vue对象, 最好别使用箭头函数, 因为此时的this为undefined,
    通常会添加self:this 属性来获取当前vue对象, 并在函数里面使用self来获取vue对象.

#### 1.3.13 vue脚手架3.0版本之前的路由配置
* vue router插件必须在src目录下(第一层)
#### 1.3.14 前端生成excel表格
npm插件包: Track to this [plug](https://www.npmjs.com/package/export-excel-eug)
插件包源码: Track to this [repository](https://github.com/EugeneHuang9638/export-excel-eug)
测试包: Track to this [test repository](https://github.com/EugeneHuang9638/test-export-excel-eug)
#### 1.3.15 限制输入字符的语句在linux中会失效
* 使用 return (/[\d]/.test(String.fromCharCode(ev.keyCode || ev.which))) || ev.which === 8 的方式限制输入字符, 在window环境上是可行的, 但是在linux系统下会失效
#### 1.3.15 vue.js嵌套路由 子路由path的定义
* vue.js 嵌套路由 chidren中的path不需要加斜杠(/)
  ```js
    {
      path: '/user',
      component: () => import('具体的组件'),
      children: [
        {
          path: 'list',
          name: 'user-index',
          component: () => import('具体的组件')
        }
      ]
    }
  ```

#### 1.3.16 Nuxt.js 官网提供的自定义loading组件. 并将该组件定义在nuxt.config.js的loading 选项中
* 组件
  ```js
    <template>
      <el-container class="loading-container" v-show="loading">
        <el-main class="loading-main" v-loading="true"
          element-loading-text="加载中"
          element-loading-spinner="el-icon-loading"
          element-loading-background="rgba(0, 0, 0, 0.3)"></el-main>
      </el-container>
    </template>

    <script>
    export default {
      data: () => ({
        loading: false
      }),
      methods: {
        start () { // 可以理解成钩子函数, 路由更新时被调用
          this.loading = true
        },
        finish () { // 路由更新完毕(asyncData方法调用完成且页面加载完)是被调用
          this.loading = false
        },
        fail () { // 路由更新失败时调用
        }
      }
    }
    </script>
  ```
* 配置 
  ```js
      /*
      ** Customize the progress-bar color
      */
      loading: '@/components/loading.vue', // 自定义loading组件的位置
  ```

#### 1.3.17 vue.js父子组件加载顺序
* 从上往下查看

|  父组件  |  子组件  |
| -------- | ------  |
|   beforeCreate   |         |
|   created   |         |
|   beforeMount   |         |
|      |    beforeCreate    |
|      |     created    |
|      |    beforeMount     |
|      |     mounted    |
|   mounted   |         |
|    beforeUpdate(可获取渲染之前的dom元素)    |  beforeUpdate  |
|    update(可获取最新的dom元素)    |  update  |
|      |    beforeDestroy(有vue实例)     |
|      |    子组件destroyed(无vue实例)     |
|   父组件beforeDestroy   |         |
|   父组件destroyed    |         |

#### 1.3.18 vue.js .sync修饰符
* 背景: 都知道在编写vue组件的时候只能使用一个v-model 完成双向数据绑定, 若想绑定多个双向数据绑定的变量呢？
* 解决方案: 使用.sync修饰符  
    1. 父组件parent.vue   
      ```
        <children v-model="value" :customerAttr.sync="myValue" />
      ```
    2. 子组件chirldren.vue  
      ```
        methods: {
          notify (valueInner) {
            this.$emit("update:customerAttr", valueInner)
          }
        }
      ```   
      => 当在子组件中调用了notify方法时, 则会同时更新父组件的myValue的值为子组件$emit中的valueInner

### 1.4 ElementUI
### 1.5 npm
#### 1.5.1 package.lock.json
```
npm 5.6之后是以package.lock.json的版本为主, 5.1之前package.lock.json基本上没啥用, 因为就算指定了版本但还是会install最新的
```
#### 1.5.2 package.json文件中的依赖
```
后面使用的是^符号(eg: ^2.0.0)的话, 如果依赖包更新了 那么会下载最新的依赖(前提, package.lock.json中没把版本定死),
若确定是使用某个依赖包的话, 那么使用~符号  eg: ~2.0.0  则只会下载2.0.0版本的依赖
```
#### 1.5.3 npm install指定版本依赖并保存至package.json
* eg: 安装前端生成excel表的依赖 xlsx: 0.14.0
```npm
npm install --save xlsx@0.14.0
npm install --save file-saver@2.0.0
```

#### 1.5.4 npm发布自己编写的vue.js组件库
1. 使用vue3.0版本之前的脚手架, 搭建webpack-simple模板
   ```
      vue init webpack-simple export-excel-eug
   ```
2. 修改webpack.config.js文件, 配置别名 '@': resolve('src')
   ```
    个人习惯, 习惯于使用@与根目录进行映射
   ```
3. 撰写自定义组件
4. 调用Vue.component api全局注册组件
5. 修改webpack.config.js文件, 修改打包配置
   ```
    * output配置: 
      1. 新增library="exportExcel"  -> // 模块名, 其他类库使用require的方式引用的原因就是配置了这个
      2. 新增libraryTarget="umd" -> // libraryTarget会生成不同umd的代码,可以只是commonjs标准的，也可以是指amd标准的，也可以只是通过script标签引入的
      3. 新增umdNamedDefine="true" -> // 会对 UMD 的构建过程中的 AMD 模块进行命名。否则就使用匿名的 define
      4. 修改filename为exportExcel.js
    ```
6. 修改package.json文件, 指定插件入口  
   ```
      "private": false,  -> 需要发布, 因此需要将这个字段改为 false
      "main": "dist/exportExcelEug.js",  -> 当在第三方使用类库, 使用 import ExportExcelEug from 'export-excel-eug'时, 会根据插件的package.json的main入口找文件
   ```
   ```
    library：指定的就是你使用require时的模块名
    libraryTarget：
      为了支持多种使用场景，我们需要选择合适的打包格式。常见的打包格式有 CMD、AMD、UMD，CMD只能在 Node 环境执行，AMD 只能在浏览器端执行，UMD 同时支持两种执行环境。显而易见，我们应该选择 UMD 格式。
      有时我们想开发一个库，如lodash，underscore这些工具库，这些库既可以用commonjs和amd方式使用也可以用script方式引入。
      这时候我们需要借助library和libraryTarget，我们只需要用ES6来编写代码，编译成通用的UMD就交给webpack了
    umdNamedDefine：会对 UMD 的构建过程中的 AMD 模块进行命名。否则就使用匿名的 define
   ```
7. 由于插件的指定路口在dist打包目录下, 所以先把包打好再发布
8. 遇到的坑

    |  错误  |  原因  |
    | ----   |  ---- |
    | no_perms Private mode enable, only admin can publish this module | 默认镜像非官方的, 需要重新设置.命令: npm config set registry http://registry.npmjs.org　|  
    | npm publish failed put 500 unexpected status code 401 | 没有登录，需要登录: npm login 即可|  
    | npm ERR! you do not have permission to publish “your module name”. Are you logged in as the correct user? | 包名被占用, 需要重新命名. 命名之前最好先去npm官网查看包名是否被占用 |  
    | You cannot publish over the previously published versions | 每次发布时需要更新版本, 修改package.json文件的version字段即可.| 
    | npm publish时经常报403 | 可以确认下注册的账号是否在邮箱中验证完毕 |
9. 发布包的一句核心话就是: 将所有的插件(插件存在install方法)export出去, 并在使用组件项目入口使用Vue.use(插件)的方式   
   (Vue.use方法时会触发插件的install方法)生效.

   [附带详细教程](https://www.imooc.com/article/19691)

#### 1.5.5 npm+git搭建私有npm仓库
* 背景: 当项目中有自己内部写好一些类库, 但是不想发布到npm公网中, 搭建私有仓库为不二选择。
* 搭建npm私有仓库的三种方式:
    1. cnpm搭建
    2. verdaccio搭建
    3. git

    ```
      每种方式都自己的优劣势, 感兴趣可以自己研究。
    ```
* npm + git搭建私有仓库
    1. 选择该方式原因
       ```shell
         npm + git 搭建、集成速度快
       ```
    2. 创建私有git仓库(最好是创建一个npm私有仓库的group, 易于管理。 注:gitlab中能创建group以及私有仓库, github不能创建group, 且私有仓库需要付费)
       ```
         假设在git上创建了一个group, 叫npm-pr, 私有仓库名为hello-world。
         url为http://host/npm-pr/hello-world.git 或 git@host:npm-pr/hello-world.git
       ```
    3. 初始化scope
       ```shell
         npm init --scope=npm-pr
       ```
    4. push代码

    ***
    上述4步算完成私有仓库的搭建

    5. 项目依赖类库, 从私有仓库中获取(package.json文件中配置)
       ```json
        // 采用ssh的方式拉取指定branch的依赖
        "dependencies": {
          "@npm-pr/hello-world": "git+ssh://git@host:npm-pr/hello-world.git#branchName"
        },

        // 采用https的方式拉取指定branch的依赖
        "dependencies": {
          "@npm-pr/hello-world": "git+https://用户名:密码@host:npm-pr/hello-world.git#branchName"
        },
       ```
    6. 安装依赖
       ```shell
         npm install @npm-pr/hello-world

         # 安装后的包路径为node_modules/npm-pr/hello-world  所以在对应前端框架引用插件入口出要注意文件的位置
       ```

### 1.6 Html
#### 1.6.1 手动设置ie浏览器以最新版本渲染页面
* 添加meta,使IE用最新版本渲染页面
```html
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
```
#### 1.6.2 指定浏览器对html文件的编码格式
* HTML 页面, 在head标签的meta标签中设置charset='utf-8' 就能使浏览器以utf-8的标准去解码
```html
<meta charset="UTF-8">
```

### 1.7 ES6语法
#### 1.7.1 export 和 export default的区别
1. 首先, ES6中存在多模块的概念, 相当于java中的pacakge, 在使用它的时候需要import,  
   但是它不同与java的package的是, 它需要手动export出去, 即将包暴露出去
2. export default 只能暴露出一个接口.
   eg: xxx.js文件
   export default class xxx {
     static a = 'attribute'
     static f = () => {console.log('f')}
   } 
   xxx中包含许多属性和方法, 且需要static修饰.
   
   使用时:
     import xxx from 'xxx文件的路径'
     获取a属性: xxx.a
     调用f方法: xxx.f()
3. export 通常是可以暴露多个接口, 但是在import时, 需要加上 {} 来import指定的接口
   eg: xxx.js文件:
   const a = 'attribute'
   const f = () => {console.log('f')}
   export {
     a,
     f
   }

   使用时:
     获取a属性: import { a } from 'xxx文件路径'
     获取f方法: import { f } from 'xxx文件路径'
     同时获取a属性和f方法: import { a, f } from 'xxx文件路径'

***

## 二. 后端
### 2.1 Java basic
#### 2.1.1 Double引发的Null Pointer Exception
```java
Double amount = null;
amount += 123;  --> Null pointer exception , 底层后调用 amount.valueOf() + 123  进而导致NullPointerException
```
#### 2.1.2 强转类型前提
* Java不能直接使用(Long)的方式将integer类型强转成Long类型. 因为Integer和Long两个类没有继承关系。
    ----->  只有存在继承关系的两个类才能使用括号的方式进行强转。
#### 2.1.3 基础数据类型相等的判断
* 最好使用包装类型并使用equals方法进行判断, 拿Integer和Long类型举例,在(-128 ~ 127)的范围内,是从缓存中取数据, 当不在这个范围内时, 每次都是创建新对象. 栈内存中存放对象引用地址不一致, 使用 == 来判断相等时, 当然不一致。
#### 2.1.4 Split方法
* java split方法, 这种字符串切割 "a, b, c," 若单独的使用split(",")的方式  
  那么最后的数组长度为3而不是4, 因为这会调用split一个参数的重载方法, 
  可以指定长度 split(",", 4) 则指定长度为4
#### 2.1.5 异常中try, finally, catch中return的顺序
* 前提: 程序抛了异常, 并且try catch住了.
1. 在catch中有return,finally中无return:  
   会先执行catch中的所有语句, 包括return后面的逻辑, 执行完之后不会立刻return, 而是去找有没有finally,
   如果有则执行finally的语句, 再返回到catch中的return
2. catch和finally中都有return:  
   会先执行catch中的所有语句, 包括return后面的逻辑, 执行完之后不会立刻return, 再进finally, 此时发现
   finally中有return, 那么就会走finally中的return逻辑, 从而catch中的return失效了, 即出口在finally了
#### 2.1.6 Servlet中没有暴露出无参构造器(手动编写了带参构造器)
* 访问时会报500, 因为系统会采用反射的机制调用无参构造器初始化当前servlet
#### 2.1.7 根据oss url获取远程图片, 并转成base64
1. 使用ossClient的getObject方法获取图片的输入流
2. 使用1024字节长度的方式, 读取输入流的信息, 并同时写进ByteArrayOutputStream输出流
     ``` java
        ByteArrayOutputStream outStream = new ByteArrayOutputStream();
        int len = 0;
        while ((len = ossObject.getObjectContent().read(buffer)) != -1) {
            outStream.write(buffer, 0, len);
        }
     ```
3. 再将输出流转成byte数组
	    outStream.toByteArray()
4. 使用jdk自带的Base64 encode编码方法, 将byte数组转成base64

* 使用字节限制每次读取的长度, 使用while循环保证能读取整个流

#### 2.1.8 动态代理抛出实际真实异常
* 因为动态代理对象抛出的异常对象为顶级对象Throwable, 所以要获取真实对象的话, 需要调用异常的e.getCause()方法

#### 2.1.9 多线程基础
##### 2.1.9.1 volatile关键字与System.out.print的欢喜冤家
* volatile关键字的作用大家也都明白, 大致就是提供多线程对临界区变量的可见性、一致性和有序性(JMM主要围绕这三个特性: Java内存模型)
  在 `实战Java并发程序基础`一书中有提到, 当jvm采用server模式运行java程序时, 由于`配置比较高大上(暂时先这么理解)`, 导致jvm有闲
  情进而导致cpu有闲情对系统进行优化, 尽量让所有的临界区的变量变得可见。
* 上面的背景只是就先介绍到这里, 咱们看下面一段代码: 
  ```java
    public class Thread9 {
      private static boolean ready;
      private static int number;

      public static class ReaderThread extends Thread {

          @Override
          public void run() {
              while(!ready);

              System.out.println("死循环结束, number = " + number);
          }
      }

      public static void main(String[] args) throws InterruptedException {

        new ReaderThread().start();
        Thread.sleep(1000);
        number = 43;
        ready = true;
        System.out.println("主线程休息3秒");
        Thread.sleep(3000);
      }
    }

    /* 
      针对如上的理解, 我们可以得知, 开启ReaderThread线程时, 在主线程睡眠1秒时, ReaderThread线程一直处于死循环中,
      当主线程修改临界区number和ready的变量时, 由于ReaderThread线程一直处于死循环中, 压根没给jvm留出一丝的空闲
      时间, 所以jvm没法对系统进行优化，尽量让所有的临界区的变量变得可见, 所以上述代码运行结果位: ===>  
        控制台输出 "主线程休息3秒" 并程序一直在运行中, 给人的感觉就是无任何反应
    
       ==>  若想让线程能够执行完毕, 则只需要在ready变量添加volatile标识符进行修饰即可。


       同时：还有一种能让人意想不到的方法, 在ReaderThread线程的run方法的死循环中, 添加System.out.print()输出语句,
            输出任何信息都行, 你会发现我不添加volatile标识符, 线程也能正常结束！！！！

            这是为什么呢？？？

            ==>  原因就在于System.out.print()源码中有synchronized关键字, 对于jvm而言, 有synchronized关键字的是需要
                 获取和释放对象的锁的, 这些操作对于jvm而言是需要等待时间的, 而此时jvm发现我有闲情了, 那么它就会优化
                 系统代码, 尽量保证临界区的变量能够对所有线程可见, 所以线程就正常结束了。
    */
  ```
##### 2.1.9.2 JDK线程状态及转换图
![JDK线程状态及转换图](https://github.com/AvengerEug/treadpit/blob/master/jdk_thread_status.jpg)

#### 2.1.10 抽象类和接口的区别
* 抽象类
    1. 子类必须重写抽象类的`抽象`方法
    2. 包含抽象方法的一定是抽象类
    3. 不能直接实例化对象
    4. 抽象方法只有声明，无方法体，方法权限不能为private

* 接口
    1. 可以同时实现多个接口
    2. 方法都是默认public修饰的，无方法体
    3. 接口中的变量默认都是public static final修饰的常量
    4. 实现接口的类一定要实现接口中的所有方法

* 共同点
    1. 都不能实例化对象
    2. 都有抽象方法
    3. 派生类都要重写或实现抽象方法

#### 2.1.11 Overload和Override的区别
* Overload(重载)
    1. 参数个数、类型不同
    2. 与返回值和函数修饰符无关
    3. 存在于同一个类中

* Override(重写)
    1. 子类重写父类方法
    2. 方法名、参数名、参数个数、参数类型完全一致
    3. 子类方法权限不能小于父类, 方法权限 >= 父类
    4. 子类方法抛出的异常不能大于父类, 方法抛出异常 <= 父类
    5. final修饰的方法不能被重写


#### 2.1.12 ArrayList，LinkedList，Vector

| 类别     | 底层实现 | 是否线程安全 | 是否可重复 | 是否有序 | 其他
| ----| ------ | ------ | ------ | ------ | ------ 
| ArrayList |   线性表(数组)  |  `否`  |   是   |    否   |   默认容量为10，每次扩容1.5倍 + 1，查询快，新增、删除慢
| LinkedList |   链表  |  `否`   |  是  |   无  |  对于新增、删除快，查询慢
| Vector |   线性表   |  `是`   |   是   |   是   |  同ArrayList


#### 2.1.13 HashMap, HashTable, ConcurrentHashMap

|  类别   | 底层实现 | 是否线程安全 | 是否可重复 | 其他
| ----| ------ | ------ | ------ | ------
| HashMap |   ---   |  `否`   |   否   |  可允许key或值为null，实现的是Map接口
| HashTable |   ---   |  `是`   |   是   |  不允许key或值为null, 实现的是Directory接口
| ConcurrentHashMap |   --   |  `是`   |   是   |  与HashMap一致


#### 2.1.14 创建Class对象的几种方法
* 根据类加载器
    ```java
      Class c = Class.forName("包.类名");
    ```

* 根据实例对象
    ```java
      String str = new String("test");
      Class c = str.getClass();
    ```

* 根据类获取
    ```java
      Class c = String.class;
    ```

#### 2.1.15 ArrayList.asList()的坑
```java
  String strArr[] = new String[] {"a", "b"};
  List list = Arrays.asList(strArr);

  // => 此时执行list.add()方法会抛出UnsupportedOperationException异常, 因为返回的list类型为Arrays的内部类, 里面并没有重写add方法, 所以调用了父类的AbstractList add方法, 在AbstractList类中的add方法中抛出了UnsupportedOperationException异常并且执行strArr[0] = "h"  list中的第一个元素也会改变
```

#### 2.1.16 不要在 foreach 循环里进行元素的 remove/add 操作
```
  由于单线程的fail-fast机制, 当多个线程对fail-fast集合进行修改时, 可能会抛出ConcurrentModificationException  
  所以最好是通过迭代器 Iterator来操作, 利用迭代器的remove方法来进行删除
```

#### 2.1.17 JVM 类加载器
* 背景:
    ```
      我们都知道java是跨平台的，但所谓的跨平台是指编译后的class字节码文件通过jvm能运行在不同的平台上，而jvm在   
      对应平台jdk的安装过程中就已经安装完成。那么运行一个普通的java程序(eg: 控制台输出Hello World)jvm在底层   
      做了哪些事呢？
    ```
* javac命令:  
    ```
      javac命令的主要作用就是将.java后缀名文件编译成.class字节码文件, 在大多数IDE中, 这一步骤在run程序的时候   
      都帮我们完成了。
    ```
* java命令:  
    ```
      java命令就是将javac命令编译后的.class字节码文件运行起来。在此时, JVM将起着非常重要的作用。   
      首先, 一个普通无继承的类拥有四个类加载器:   
        1. 自身的classLoader:  
        2. AppClassLoader:  
            主要加载应用程序的类, 如自己编写的类、第三方jar包的类库。eg: maven中引入中的所有第三方jar包
        3. ExtClassLoader:  
            能拿到它的引用，一般加载jdk安装目录下的jre/lib/ext文件下的所有jar包。
        4. null(根类加载器):  
            在程序中拿不到它的引用，但是它实际存在，由c++编写, 根加载器一般加载比较重要的类. 比如jdk安装目录下的jre/lib/rt.jar类库(里面存放着jdk类库的字节码文件, 这就是我们能使用jdk api的原因)
    ```
* 具体java应用程序class加载时间调用顺序如下图所示:
![JDK_Classloader](https://github.com/AvengerEug/treadpit/blob/master/jvm_classloader.jpg)

### 2.2 Spring Cloud
#### 2.2.1 服务注册中心Eureka
* 服务注册中心包括Eureka和zookeeper
* 选择Eureka作为服务注册中心原因如下:
  1. Eureka完全开源, 由Netflix公司生产环境三年的更新迭代,功能和性能上都非常稳定,且社区活跃
  2. 是SpringCloud首选推荐的服务注册与发现组件
  3. 与SpringCloud的其他组件 eg: Ribbon, Hystrix, Zuul等组件能无缝对接.

* 工作角色:
  1. 服务注册中心(register Service)
  2. 服务提供者(Provider Service)
  3. 服务消费者(Consumer Service)

#### 2.2.2 ApiGateWay(Zuul)
* 选择Zuul作为路由网关的原因
  1. Zuul，Ribbon以及Eureka相结合，可以实现智能路由和负载均衡的功能
  2. 对外只暴露一个api端口, 由内部转发至具体服务
  3. 可以做用户身份认证和权限认证, 可以起到保护服务的作用
  4. 可以实时对请求进行日志输出
  5. 实现流量监控, 在高流量的情况下, 对服务进行降级

* 若在配置路由规则时，指定了请求的url那么zuul底层的ribbon就不会做负载均衡功能了

#### 2.2.3 FeignClient
* 解析如下FeignClient定义的代码
```java
  @FeignClient(value="service-user", configuration = FeignConfig.class)
  @RequestMapping(value = {"/users"})
  public interface UserClient {

    @RequestMapping(value = { "/{userId}/inner" }, method = RequestMethod.GET)
    FeignMessage getByIdInner(@PathVariable(value = "userId") Long userId);
  }

  /*
   1. @FeignClient(value="service-user", configuration = FeignConfig.class)
      => FeignClient的定义: 表明使用该client是，会找到service-user模块(在服务网eureka注册服务时指定的service.application.name配置)
         并配置了FeignClient的配置(FeignConfig.class), 可以添加请求拦截器已经响应拦截器
   2. @RequestMapping(value = {"/v1/users"})
      => 配置了FeignClient发送RPC请求时的requestMapping
   3. @RequestMapping(value = { "/{userId}/inner" }, method = RequestMethod.GET)
      FeignMessage getByIdInner(@PathVariable(value = "userId") Long userId);  
      => 配置了当调用geByIdInner方法时的路径, 所以当在代码中调用
         userClient.getByIdInner(1L)时. 底层会发送一个 method=GET, url=/users/1/inner 的HTTP Request,
         返回值通过自定义的FeignMessage来接收(底层会做序列化和反序列化操作)
   4. 最重要的一个点: 如何将userClient注入到Spring的IOC容器？
      => 在需要用到userClient的service的入口处添加
         @EnableFeignClients(basePackages = {"UserClient的包路径"})
         这样在服务启动时就会添加UserClient的实例至Spring IOC容器中
   */
```
* 另外, FeignClient RPC底层使用的是HTTPClient, 在传递参数的时候必须要有个顺序, 所以会将Map转成LinkedHashMap

#### 2.2.4 Swagger
* SpringCloud集成swagger
  1. 需要添加swagger依赖(所有需要暴露swagger的服务都要添加, 所以可以统一加到root的pom.xml上)
    ```xml
      <dependency>
        <groupId>io.springfox</groupId>
        <artifactId>springfox-swagger2</artifactId>
        <version>2.6.1</version>
      </dependency>

      <dependency>
        <groupId>io.springfox</groupId>
        <artifactId>springfox-swagger-ui</artifactId>
        <version>2.6.1</version>
      </dependency>
    ```
  2. 在api网关处添加swagger配置信息(添加Bean到Spring IOC容器中去)
    ```java
      @Configuration
      public class SwaggerResourcesConfiguration {

          @Primary
          @Bean
          public SwaggerResourcesProvider swaggerResourcesProvider() {
              return new SwaggerResourcesProvider() {
                  @Override
                  public List<SwaggerResource> get() {
                      List resources = new ArrayList();
                      resources.add(createResource("service-user", "service-user", "1.0"));
                      return resources;
                  }
              };
          }

          private SwaggerResource createResource(String name, String registeredEurekaServiceName, String version) {
              SwaggerResource swaggerResource = new SwaggerResource();
              swaggerResource.setName(name);
              swaggerResource.setLocation("/" + registeredEurekaServiceName + "/v1/docs");
              swaggerResource.setSwaggerVersion(version);
              return swaggerResource;
          }
      }
    ```
  3. 在ApiGateWay入口文件处添加@EnableSwagger2注解开启swagger功能

#### 2.2.5 ServerConfig
#### 2.2.6 SpringCloud常用组件及作用
* Eureka: 服务注册与发现中心, 用来存储每个服务的对应的ip和端口
* Zuul: 路由网关, 微服务api请求统一路口, 类似于nginx方向代理, 需配置一套规则才能请求到具体的服务
* Ribbon: 负载均衡, 该组件存储在ApiGateWay中, 采用轮询算法, 依次请求服务的每一个实例
* Feigh: 服务间内部调用, 底层采用动态代理, 根据feignClient接口中mvc的一些注解, 组装http请求
* Hystrix: 熔断器, 防止因某个微服务崩溃而导致整个微服务雪崩。具体内部使用采用的是每个服务走自己的线程池
### 2.3 Spring Boot
#### 2.3.1 @RequestParam 类型映射
|  后台定义类型 |  前台传数据格式 |
| -------| ------ |
|   数组类型   | value1, value2, value3   以逗号隔开 |
|   List类型   |  [value1, value2, value3]  以数组的形式 |
#### 2.3.2 @RequestMapping 方法映射关系
* @RequestMapping(value="test")  -> 在启动项目时, 框架会自动映射成/test. 最好还是加上斜杠, 规范一些。

#### 2.3.3 @RequestBody注解接收Post请求ContentType为application/x-www-form-urlencoded格式的数据
* 在通常的前后端分离项目中, 一般在前端框架使用的异步请求框架都会全局设置ContentType为application/json.
  导致在接触第三方jar包回调时遇到不同的ContentType不知如何处理
  ```
    在SpringBoot中的@RequestBody底层只有FormHttpMessageConverter支持解析application/x-www-form-urlencoded这种格式,
    但它只能将请求体中的内容转成MultiValueMap对象。
  ```
#### 2.3.4 @RequestMapping支持多种请求方法
* 注解中存在method属性, 是一个数组, 可以支持多种请求方式
    ```java
    eg: @RequestMapping(
              method = {RequestMethod.POST, RequestMethod.GET},
              value = "/user-mapping")
    ```
#### 2.3.5 @RequestMapping指定request和response的contentType
* 注解中存在consumes和produces注解属性
  前者指定request的ContentType, 后者指定response的ContentType, 属性都为数组, 支持多种类型
    ```java
    eg: @PostMapping(
              value = "/callback",
              consumes = {MediaType.APPLICATION_FORM_URLENCODED_VALUE + ";charset=UTF-8"},
              produces = {MediaType.APPLICATION_FORM_URLENCODED_VALUE + ";charset=UTF-8"})
        //指定请求和响应的ContentType为application/x-www-form-urlencoded;charset=UTF-8 的方式
    ```
#### 2.3.6 SpringBoot使用对象来接收query参数
```java
  不需要@RequestParam注解, 直接添加对象类型的参数即可.
```

#### 2.3.7 Spring mvc 全局异常处理注解@ExceptionHandler
* 该注解是方法级别的注解, 通常用来全局处理api请求时发生的异常
  所以一般会写一把BaseController并让所有的Controller都继承它, 这样就能catch到所有Controller抛出的异常

#### 2.3.8 Spring获取ioc容器上下文的两种方式
1. 通过WebApplicationContextUtil.getApplicationContext(ServletContext)的方式
   ```java
      WebApplicationContextUtil.getApplicationContext(request.getSession().getServletContext())
      // 通常需要获取tomcat容器中的HttpServletRequest对象来获取上下文,  
      // 虽然 HttpServletRequest 对象可以直接在方法里将该对象注入进去, 但是还是引入了比较重的对象, 不推荐该方式
   ```
2. 通过ApplicationContextAware接口
   ```
      1. 创建类并实现这个接口, 添加静态的ApplicationContext类型的对象。
      2. 重写里面的方法setApplicationContext方法, 初始化ApplicationContext类型的对象
      3. 将当前类注入到Spring IOC容器中. 
      
      这样, Ioc容器对象就是上述的 静态的ApplicationContext类型的对象. 
      想要具体的bean对象, 直接调用getBean方法即可.
      (注入到Spring IOC容器中的原因: spring启动时, 若有这样的类, 将会将上下文对象注入到
      实现ApplicationContextAware接口的对象的ApplicationContext属性中去)
   ``` 

* 两种方式, 建议使用第二种。

#### 2.3.9 Spring核心
* 单例模式: 所有注入ioc容器中的对象都是单例的
* Bean工厂方法
    1. 静态工厂方法
         * 通过使用静态方法来获取实例 
    2. 实例工厂方法:
         * 通过使用非静态方法来获取实例
* Inject控制反转(常用)
    1. set方法
    2. 构造函数
* Aop
    1. Aspect(切面): 定义了切面是什么以及何时使用
       Before——在方法调用之前调用通知
       After——在方法完成之后调用通知，无论方法执行成功与否
       After-returning——在方法执行成功之后调用通知
       After-throwing——在方法抛出异常后进行通知
       Around——通知包裹了被通知的方法，在被通知的方法调用之前和调用之后执行自定义的行为
    2. Join point(连接点): 业务方面的代码, 作为连接点
    3. Advice(引入): 引入允许我们向现有的类中添加方法或属性
    4. Pointcut(切点): 切点定义了“何处”需要执行code, 即表达式定义。 切点会匹配通知所要织入的一个或者多个连接点
* Annotation

#### 2.3.10 Spring bean生命周期
* singleton: 单例模式, 默认。只存在一个实例
* propytype: 原型。每次注入属性时都是new一个新对象
* request: 针对每次http请求, 都会new一个新对象, 适用于WebApplicationContext环境
* session: 每次会话都会new一个新对象, 同一次会话共用一个实例
* global-session: 所有会话共用一个实例

#### 2.3.11 SpringBoot是job注解和异步调用注解生效前提
* 异步注解:  @Async
    要使注解生效, 需要在入口处添加@EnableAsync注解
* job注解: @Scheduled  
    要使job定时器生效, 需要在入口处添加@EnableScheduling注解

#### 2.3.12 Springboot yml文件配置的坑
* 在2.0.5.RELEASE版本中(其它版本没有测试)若使用key为no/yes时, load到内存中的key会发生变化
  eg: 存在这样一个配置
      product:
        no: product_01
        yes: product_02
      
      spring在将配置文件load到内存后, 使用@Value("${product.no}")的方式是会报错的: 报无这样的key
      为啥呢？ 因为spring会将key load成 product[false] 或 product[true]

#### 2.3.13 @Autowired和@Resource的区别
* @Autowired: 默认按照byType的方式进行bean匹配, 是spring框架中的注解
* @Resource: 默认按照byName的方式进行bean匹配, 是jdk中自带的注解

#### 2.3.14 SpringBoot默认包扫描路径
* 默认包扫描路径为Springboot项目入口类所在包及子包，所以如果项目中会依赖一些common的jar包, 并且jar包中包含一些
  springboot的注解时, 必须要保证依赖common包的路径能被springboot扫描注解时扫描到
  
  eg: 
    ```
      假设一个springboot项目依赖一个jar包, 其中这个jar包会存在一个spring 上下文的工具类(一般用于因加载顺序无法
      进行依赖注入属性时, 会用它来获取spring管理的bean, 通常是实现ApplicationContextAware接口)。 当在使用redis
      作为mybatis的二级缓存时, 需要对实现mybatis Cache接口的类添加redisTemplate类型的对象, 并重写一些方法,
      此时redisTemplate是无法依赖注入进去的。 此时就会通过获取spring上下文的工具类来获取bean, 所以此时若该工具类
      存在实例化bean的相关注解时, 必须保证该类会在springboot的包扫描有效路径下。
      
      不仅是在这种case下, 比如说在过滤器、拦截器中要注入一些属性时, 也是会注入失败的(因为过滤器或者拦截器加载的时
      间是在spring上下文之前的), 此时必须要依赖spring上下文来获取bean对象。
    ```
  

### 2.4 Mybatis
#### 2.4.1 parameterType为int/long时, 参数为0的处理
* 若传入的参数为0, mybatis会将它当成```空字符串```处理, 所以会查出name为空字符串的数据
  ```xml
  <select id="countApplicant" parameterType="int" resultType="long">
      <![CDATA[
          SELECT COUNT(1)
          FROM applicant
          WHERE name = #{parameter}
      ]]>
  </select>
  ```

#### 2.4.2 $和#区别
* $会存在sql注入的风险, #不会。 因为$是将数据和sql语句一起编译的 而#是先编译sql语句再将数据绑定上去, 即跟原生jdbc的问号占位符一样(?, ?, ?....)
* 所以通常在模糊模糊查找时会添加bind标签将需要模糊查找的key预先编译好, 再直接用#将bind定义的变量keywordWrapper进行筛选即可,。
  ```XML
    <bind name="keywordWrapper" value="keyword + '%'"/>

    <![CDATA[
      SELECT * FROM user WHERE name LIKE #{keywordWrapper}
    ]]>
  ```

#### 2.4.3 ORM映射文件 type和map后缀的区别
1. parameterType和parameterMap
  * parameterType指的是传递进去的参数类型, 基本数据类型以及pojo类型(map或类对象)
  * parameterMap 一般很少用, 懒得研究
2. resultMap和resultType
  * resultType 返回基本数据类型
  * resultMap 返回对象类型, 同时该对象需要在xml文件中配置model与db字段的映射关系

#### 2.4.4 Mybatis resultMap中type=map, 使用枚举的typeHandler前提
* 需要在字段中添加javaType类型, 指定具体的枚举类是什么, 否则直接使用typeHandler会抛出
  Object does not represent an enum type的异常
  ```xml
    <resultMap id="demoMap" type="map">
        <result column="user_id" property="userId"/>
        <result column="status" property="status" javaType="枚举的具体类的class路径" typeHandler="org.apache.ibatis.type.EnumOrdinalTypeHandler"/>
        <result column="age" property="age"/>
    </resultMap>
  ```

#### 2.4.5 使用springboot 通过继承SqlSessionDaoSupport类集成mybatis
* 必须重写setSqlSessionTemplate或者setSqlSessionFactory方法, 同时在方法中添加``@Autowire``注解来开启mybatis功能(注入sqlSessionTemplate)，
  否则会抛初始化sqlSessionTemplate相关的异常

### 2.5 MySql
#### 2.5.1 export database/table command
```mysql
mysqldump -h host -u username -p database > target file

eg: 导出指定服务器(127.0.0.1)的test数据库到本地 test_local.sql 文件
    mysqldump -h 127.0.0.1 -u root -p test > c:\test_local.sql

eg: 导出指定服务器(127.0.0.1)的test数据库的user表到本地 test_user.sql 文件
    mysqldump -h 127.0.0.1 -u root -p test user > c:\test_user.sql
```
#### 2.5.2 import database/table command
```mysql
mysql --default-character-set=utf8 -h host -u username -p database > source file

eg: 将c盘根目录下test数据库的sql文件test_local.sql 导入本地test_local数据库
    mysql --default-character-set=utf8 -u root -p test_local < c:\test_local.sql
    或者登录到mysql(登录时需指定与sql文件同编码格式)并指定db 使用source命令
eg: mysql --default-character-set=utf8 -u root -p test_local
    source c:\test_local.sql

eg: 将c盘根目录下的test_user.sql表导入本地test_local数据库user表
    mysql --default-character-set=utf8 -u root -p test_local user < c:\test_user.sql
    或者登录到mysql(登录时需指定与sql文件同编码格式)并指定db 使用source命令
eg: mysql --default-character-set=utf8 -u root -p test_local
    source c:\test_local.sql

ps: --default-character-set=xxx  编码格式具体根据导出的db时选择的编码一致
```
#### 2.5.3 mysql压缩版本()启动步骤
```mysql
  A. 配置mysql bin目录的环境变量
  B. 执行mysqld --initialize-insecure --user=mysql  (若执行时报xxxx120.dll文件不存在, 则需下载vcredist_x64.exe并安装)
  C. 执行mysqld -install   -> 安装服务
  D. 执行net start mysql   -> 启动服务
  E. 默认用户名是root 无密码
```
#### 2.5.5 存储过程
* 语法:
  ```mysql
    DELIMITER $$
    DROP PROCEDURE IF EXISTS testProc2$$
    CREATE PROCEDURE testProc2()
    BEGIN
      DECLARE username INT;
      DECLARE done INT DEFAULT 0; -- 定义一个done变量, 用来判断cursor是否继续循环
      DECLARE my_cur CURSOR FOR SELECT `name` FROM `info`;
      DECLARE CONTINUE HANDLER FOR NOT FOUND SET done = true; -- 如果游标FETCH NEXT无数据了的话, 那么就会设置done为true
      OPEN my_cur;
        FETCH my_cur INTO username;
        WHILE(NOT done) DO
          INSERT INTO user_info(username) VALUES(username);
          FETCH my_cur INTO username;
        END WHILE;
      CLOSE my_cur;
    END;
    $$
    DELIMITER ;
  ```
  注意: 
  1. 存储过程内定义的变量尽量不与需要操作的表的字段一致, 否则会将表中的字段的值填充到变量中.
  2. 一般使用存储过程的场景为:
      * 需要频繁操作同一个sql语句. eg: 在权限表中, 每添加一个权限就需要将该权限与超级管理员关联起来. 此时可以创建一个将权限关联至超级管理员的存储过程
      * 当更新表字段需要同一个表中的字段作为条件时(mysql会报错``` #1093 - You can't specify target table 'xxxx' for update in FROM clause ```).
        意思就是: 不能先select出同一表中的某些值，再update这个表(在同一语句中)
        当然也可以采用嵌套子查询的方式解决, 即将select出来的结果当作一个视图, 再将视图作为条件更新表字段

#### 2.5.6 DML和DDL概念
  ```
    DDL(DATA DEFINITAION LANGUAGE 数据定义语言): 使用范围: 对database, table有操作 eg: ALTER DROP CREATE
    DML(DATA MANIPULATION LANGUAGE 数据操纵语言): 使用范围: 对数据的操作 update,create,insert,delete,存储过程, 视图等等
  ```
#### 2.5.7 mysql连接数不够
* 背景: 当整个团队集体开发某个需求时, 通常会选择一个人的db作为服务器db, 此时容易造成数据库连接池不够
解决方案:
  ```mysql
    -- 查看数据库最大连接数
    SHOW variables LIKE '%max_connections%';

    * 方案1:
    -- 重新设置全局最大链接数变量
    SET GLOBAL max_connections=1024;

    但，这种方式在重启mysql服务时就会失效

    * 方案2:
    修改mysql配置文件my.cnf，在[mysqld]段中添加或修改max_connections值：
    max_connections=1024
  ```
#### 2.5.8 flyway
#### 2.5.9 mysql sql优化
* 前提: 首先得找出哪些sql需要被优化
  ```
    步骤:  
      1. 开启慢查询sql日志功能: SET GLOBAL slow_query_log = 1(可提前查看是否开启: SHOW VARIABLES LIKE '%slow_query_log%');  
      2. 设置慢sql记录的阈值: SET GLOBAL long_query_time = 2;(查询超过两秒的sql都会记录到日志中去)  
         注意: 可能设置后执行 SHOW GLOBAL VARIABLES LIKE 'long_query_time'; 不会看到修改后的结果, 此时需重新开启一个连接才能看到  
      3. 设置日志存储位置: SET GLOBAL slow_query_log_file = 'c:\\mysql-slow.log';(或者使用默认的: SHOW VARIABLES LIKE '%slow_query_log_file%')  
      4. 查看慢查询日志
      5. 统计有多少条慢sql: SHOW GLOBAL STATUS LIKE 'slow_queries';
  ```

* 使用Explain分析sql
  ```
    语法:  EXPLAIN SQL语句
  ```
  Explain的具体分析可参考: https://www.cnblogs.com/dwlovelife/p/11110215.html

### 2.6 Elasticsearch
#### 2.6.1 linux构建es的坑
```shell
  1. es目录不能在 root下或root的子目录下
  2. 需要添加JAVA_HOME环境变量  (/etc/profile文件)
  3. 需要添加用户组, 并添加普通用户, 并给普通用户设置es文件夹的使用(可读)权限  chown -R 用户组:用户 es文件夹目录
  4. 必须使用普通用户启动elasticsearch(使用'su 用户' 命令切换用户)
  5. 根据官网提示, 因为elasticsearch是使用java编写的, 至少需要java1.8版本支持, 最好使用java1.8.0_131版本
  6. 服务器内存小的机器, 需要修改elasticsearch的config/elasticsearch.yml文件修改对内存大小 -Xms128 -Xmx512m  (其实就是启动java程序限制了堆内存最小值和最大值)
  7. 修改config文件夹下的elasticsearch.yml文件 自定义配置文件中的cluster.name(建议直接去掉前面的注释), node.name(建议直接去掉前面的注释), netword.host
     (建议使用0.0.0.0, 该配置会允许外网访问), http.port(建议直接去掉前面的注释)等配置
  8. 配置运行时环境内存大小: 
     服务器运行内存比较小的 => 修改config文件夹下的jvm.options文件, 只指定最小堆内存-Xmx512m  最大堆内存设置去掉.
     编辑 /etc/security/limits.conf文件, 修改(此文件修改后需要重新登录用户才会生效)
      * soft nofile 65535  -> * soft nofile 65536 (限制线程同时打开文件数)
         =>  注销重新登录后 输入命令验证是否生效:
         ulimit -Hn, ulimit -Sn
      * hard nproc 4096 -> * hard nproc 4096 (限制同时开启线程的最大数)
         => 注销重新登录后 输入命令验证是否生效:
         ulimit -Hu, ulimit -Su
    
      具体可参考 https://www.cnblogs.com/yesuuu/p/6962340.html
     编辑/etc/sysctl.conf 追加以下内容: vm.max_map_count=655360 保存后运行 sysctl -p 命令检验是否添加成功
  9. es搭建环境内容太小、线程数太小等常见问题: https://www.cnblogs.com/zhi-leaf/p/8484337.html
  10. logstash版本要与elasticsearch版本一致
```
### 2.7 Redis
#### 2.7.1 手动暂时性的设置密码
```shell
  config set requirepass 1234
```
* 一般不推荐这样做, 推荐直接修改配置文件
#### 2.7.2 redis配置远程支持连接
* 配置文件中,network中的修改 bind: 0.0.0.0
### 2.8 Maven
#### 2.8.1 install maven仓库找不到的jar包
```shell
mvn install:install-file -Dfile=需要install到本地仓库的jar包路径 -DgroupId=jar包的groupId -DartifactId=jar包的artifactId -Dversion=jar包的版本 -Dpackaging=jar

eg: 手动安装```c:\common-auth-0.0.1-SNAPSHOT.jar```
mvn install:install-file -Dfile=c\common-auth-0.0.1-SNAPSHOT-core.jar -DgroupId=com.cloud -DartifactId=common-auth -Dversion=0.0.1-SNAPSHOT -Dpackaging=jar

```
#### 2.8.2 maven profiles集成springboot build多环境
```xml
在父(根)pom.xml文件添加如下配置:
<profiles>
  <!-- 该配置文件主要作用是设置 默认使用的文件夹, 由activeByDefault标签决定, 随后也能支持在用maven命令build时指定环境信息  
      eg: mvn clean package -P dev  则会使用dev文件夹下的配置文件
  -->
  <profile>
    <id>local</id>
    <properties>
      <conf.active>local</conf.active>
    </properties>
    <activation>
      <activeByDefault>true</activeByDefault>
    </activation>
  </profile>

  <profile>
    <id>dev</id>
    <properties>
      <conf.active>dev</conf.active>
    </properties>
    <activation>
      <activeByDefault>false</activeByDefault>
    </activation>
  </profile>
</profiles>
     
<build>
  <resources>
    <resource>
      <!-- 存放配置文件的目录, 将conf文件夹导出到内存 -->
      <directory>src/main/resources</directory>
        <excludes>
          <exclude>conf</exclude>
        </excludes>
      </resource>

      <resource>
        <!-- 使用生效的目录 eg: src/main/resources/conf/local  => 即使用local文件夹下的applicantion.yml/property 配置文件 -->
        <directory>src/main/resources/conf/${conf.active}</directory>
      </resource>
  </resources>
</build>

---------------------------------------------------------------------

在子模块中的pom.xml文件添加如下配置:
<plugins>
  <plugin>
    <!-- springboot项目集成maven 插件. 注意:
        如果在用maven构建多模块项目时，不要将此插件放到parent pom中，否则如果有sub module不是spring boot应用,  
        在打包时就会出错。只将该插件添加到是spring boot项目的子模块, ps: plugins标签在build标签里面 -->
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-maven-plugin</artifactId>
  </plugin>
</plugins>
```
#### 2.8.3 maven pom文件scope解析
* compile: 缺省值，适用于所有阶段，会随着项目一起发布。 
* provided: 目标容器已经提供了这个artifact。所以在打包的时候该jar包不会被打进去。
* runtime，只在运行时使用，如JDBC驱动，适用运行和测试阶段。
* test，只在测试时使用，用于编译和运行测试代码。不会随项目发布。
* system，类似provided，需要显式提供包含依赖的jar，Maven不会在Repository中查找它。

#### 2.8.4 maven项目打包类型
```xml
  <packaging>pom</packaging>   -> 父类型都为pom类型
  <packaging>jar</packaging>   -> 内部调用或者作服务使用, 打成jar包
  <packaging>war</packaging>   -> 需要部署的项目
```
* maven父项目指定了version版本号后, 在依赖的子项目中,加入parent标签, 并将父模块的groupId、artifactId、version、relativePath指定后, 若子模块没有指定版本号, 则会继承父类的版本号. 若指定了, 则使用自己的, 否则使用父类的

#### 2.8.5 maven代码混淆插件导致spring 创建的bean找不到类型
```java
  后台代码使用maven build代码混淆后, 最好是在spring bean 容器创建bean的时候指定名称, 并在注入时使用同样的名称,  
  尤其是配置类, 在为配置类创建bean时指定bean的name(eg: @Componet(value="test")), 在使用  
  @Resource注解时要指定name为test(eg: @Resource(name="test")),  
  否则可能会遇到这种情况: Bean named 'XXX' is expected to be of type 'TTT' but was actually of type 'TTT'

  若使用@Autowired注入属性, 不会出现上述问题
```

### 2.9 Git
#### 2.9.1 回退版本
* git reset --hard HEAD~N  或  git reset --hard commitId~
* git reset --soft HEAD~N  或  git reset --soft commitId~
```
区别: 
  1. --hard回退到指定版本, 并直接将当前版本与回退版本之间的commit给忽略掉(输入git status命令只会看到落后版本的提示)
  2. --soft回退到指定版本, 会将当前版本与回退版本之间的commit给缓存到寄存区(输入git status命令可以看到所有回退的所有改动)

解释下 '~':
  在git中HEAD表示的是当前版本, 而~表示的是包含指定版本(CommitId), 所以HEAD~的意思就是包含当前版本(CommitId)
  但同时~后面可以接数字, 表示包含当前版本的前面N个版本, eg HEAD~2 表示包含当前版本的前面2个版本
```
#### 2.9.2 查看分支树
  ```
    git log --graph --pretty=oneline --abbrev-commit
  ```
#### 2.9.3 只查看commitId和comments的背景
  在自动化部署时, 通常会将最新的commitId(前6位)作为镜像的tag, 若需要确定自己的代码有没有上环境时, 可以根据镜像的tag和commit来确认,
  但``` git log ```命令呈现的东西太多, 提供给我们想要的信息(commitId)太少, 所以可以使用如下命令查看更多的commitId
  ``` git log --pretty=oneline ```, 当然也可以使用linux管道流关键字(grep)进行commit定位 ``` git log --pretty=oneline | grep 112233```
#### 2.9.4 cherry-pick和merge的区别
  ```
    主要区别在于整个项目流水线:   
      1. 使用cherry-pick的方式将某个提交应用到当前分支和在当前分支修改代码提交代码一致.
      2. 使用merge的方式在流水线会多一个分支.
  ```
![cherry-pick&merge区别](https://github.com/EugeneHuang9638/treadpit/blob/master/git-cherry-pick%26merge.jpg)
#### 2.9.5 合并commit
背景: 合并commit有益于管理整个项目, 对于一个issue, 一个小模块应该是只包含一个commit, 这样能清晰的看到代码的改动
命令: git rebase -i commitId~  或 git rebase -i HEAD~N
      与[回退版本](#281-回退版本)的操作差不多, 选择需要合并的commitId即可
      在rebase界面根据页面的提示操作即可
      完成rebase操作后需要强制push代码, 所以此操作有风险, 一定要本地的代码是最新的. 
#### 2.9.6 git reset HEAD~ 带来的坑
  ```
    首先我想操作的是想把某个被add进去的文件给reset回来, 结果操作成 git reset HEAD~ 了
    最后执行的结果就是, 将我本地的改动和当前分支的最新的一次提交的改动给合并了. 导致分支的commit
    回退到最新提交的上一个版本. 所以此时我本地的改动乱了. 
    
    为啥会出现这样的情况?
    首先, HEAD关键字是分支上当前的指针, git reset HEAD 命令后面如果接的是文件, 效果是能和我的初衷一样的, 
    但是如果后面加的是~的话, 那么就会将某次提交的改动回退.而正巧 HEAD~ 和HEAD~1 是一样的(即
    HEAD~默认会在~后面加一个数字1), 所以 git reset HEAD~n  比 git reset --soft commitId~/HEAD~n 更强.
    因为前者是将commit回退 并将改动与本地的改动合并. 而后者是将commit回退, 但是将改动放入寄存区(git add后的区域)
    如果要将改动与本地的改动合并的话 还要多执行一个 git reset . 操作.
  ```
#### 2.9.7 Github中提交的记录在Contribution中看不到
* 原因: 记录是提交了, 但是author与git中的用户名和邮箱不一致  
* 解决方案:  
    1. git log 查看命令找到想要在Contribution生效的提交  
    2. 执行git rebase -i -p commitId~  =>  与合并commit类似, 找到一个范围  
    3. 进入修改页面, 将需要修改author信息的commit前面的pick修改成edit或者e
    4. 保存退出(windows: Esc + : + wq + 回车)
    5. 重新设置author信息: git commit --amend --author="AvengerEug <eugenesumarry@163.com>"  
       包括用户名和邮箱
    6. 执行: git rebase --continue 完成当前commit信息的修改.  
    Notes:
       若commitId和HEAD指针包含的commit较多  
       则需要重复执行 3-6步  
* 若想支持以后的提交都能生效, 则需要全局配置git的用户名和密码  
* 若想针对单个项目生效则在对应的仓库中执行如下代码:  
    git config user.name "xxxx"  
    git config user.email "liu@example.com"  
* 具体可参考[此](https://www.jianshu.com/p/72717f1a1e90)


### 2.10 设计模式与应用
#### 2.10.1 简单工厂 + java多态性完成订单流水操作
* 参考[此项目](https://github.com/EugeneHuang9638/simple-factory)
#### 2.10.2 适配器模式 + 动态代理集成第三方类库, 完成日志记录操作
* 参考[此项目](https://github.com/EugeneHuang9638/dynamic-proxy-adapter)
#### 2.10.3 模板方法
* 参考[此项目](https://github.com/AvengerEug/template-method)
#### 2.10.4 观察者模式
* 参考[此项目](https://github.com/AvengerEug/observer)

* 注意: 
    1. 发布订阅模式中, 发布者和订阅者互不认识, 它们是通过中间件来交互的, eg: RabbitMq中的DirectExchange和   TopicExchange
    2. 观察者模式中, 发布者和订阅者是相互认识的, 他们可以直接交互, eg: RabbitMq中的FanoutExchange

***

## 三. DevOps
### 3.1 Docker
#### 3.1.1 搭建远程本地仓库
1. 下载镜像registry： docker pull registry   => 默认在registry.hub.docker.com 中拉去镜像
2. 运行镜像: docker run -itd -v /data/registry:/var/lib/registry -p 5555:5000
            --restart=always -name registry registry:latest
            
            命令解析:
              -itd: 在容器中打开一个伪终端进行交互操作, 并在后台运行
              -v 把宿主机的 /data/registry目录绑定到容器的/var/lib/registry目录(该目录是registry容器中存放镜像文件的目录), 来实现数据持久化
              -p: 映射端口, 宿主机的5555端口映射到容器的5000端口
              --restart=always: 重启策略, 假如容器异常退出会自动重启
              --name registry: 自定义容器名为registry
              registry:latest: 镜像名和tag名
3. 运行registry镜像成功后, 可以在另外一台机器创建镜像并push到该仓库中
4. 在另外一台机器中(最好是linux), 
    创建Dockerfile文件, 内容如下:
    FROM ubuntu
    AMD echo 'Hello docker!'
    
    并在与Dockerfile文件同级目录下执行 docker build -t 47.100.26.16:5555/project/vue-docker:v1 .  来build镜像, 
    或者使用docker build -t 47.100.26.16:5555/project/vue-docker:v1 Dockerfile文件的路径来build镜像
5. 执行完第4步的时候,  此时运行docker images命令 可以看到名称为47.100.26.16:5555/project/vue-docker tag为v1的镜像
6. 此时在本地新建/etc/docker/daemon.json 文件, 若该文件中已存在, 则添加 "insecure-registries: ["远程registry1仓库的ip以及端口", "远程registry2仓库的ip以及端口", '等等, 以此类推']"
    做此步骤的原因是, 若不添加 则会默认以https的请求去访问registry镜像仓库, 修改完之后需要重新加载daemon重启docker服务, 
    命令: sudo systemctl daemon-reload && sudo systemctl restart docker
    重启之后 可以执行docker info命令查看刚刚的配置有没有生效, 若能看到配置则代表生效
7. 此时可以执行push命令, 将仓库push到自己搭建的仓库了
    命令: docker push 47.100.26.16:5555/project/vue-docker:v1
8. 执行完第7步后, 可以选择在47.100.26.16机器上pull镜像或者在其他机器中pull镜像了.
    命令: docker pull 47.100.26.16:5555/project/vue-docker:v1 
    注: 若是在47.100.26.16本机上pull的话, 则可以直接把ip改成127.0.0.1或者也可以重复第六步的步骤, 将47.100.26.16:5555配置进去
        若是在没有将47.100.26.16:5555该配置配置到daemon.json文件的话, 需要额外配置一下才能拉取镜像
9. 执行镜像
    命令: docker run -d -p 8000:80 镜像名:tag  或者 docker run -d -p 8000:80 镜像Id

```
注意: 
1. 47.100.26.16远程docker仓库的公网ip, 并要开启5555公网ip
2. 制作的镜像tag名必须为 镜像仓库的url可以访问的地址.
   通常将它设置成 docker镜像仓库公网ip:公网端口/project/自定义镜像名:tag名
   目的是在执行docker push/pull命令时, 能找到远程仓库镜像的地址(规则是这样)
```

#### 3.1.2 push镜像到本地仓库
#### 3.1.3 使用ssh远程执行命令运行容器
#### 3.1.4 挂载宿主机目录
背景: 需要php运行环境运行指定项目
1. 克隆该[项目](https://github.com/richarvey/nginx-php-fpm)到本地
2. docker build -t docker-php:latest .
3. docker run -it -d -p 8002:80 -v /root/php/resource:/var/www/html docker-php:latest

```
注意:
  * clone上述指定项目时, 可以在直接使用作者提供的快速拉取和运行镜像的命令:  
    docker pull richarvey/nginx-php-fpm:latest & sudo docker run -d richarvey/nginx-php-fpm  
    这样就可以省略上述制作镜像的第二步.
  * 解析下第三条命令: 
      -it: 在容器中打开一个伪终端进行交互操作
      -d: 容器在后台运行
      -v: 挂载宿主机目录 前者为宿主机挂载目录, 后者为容器中目录 eg: -v /root/php/resource:/var/www/html
          至于为什么挂载到容器的/var/www/html目录, 由制作镜像时nginx的配置文件决定(公共资源目录: 可以通过
          ngxin直接访问资源的路径).
```
#### 3.1.5 ADD命令的坑
正常在linux系统中, cp命令或者mv命令 
eg: mv/(cp -r) ./test /root/test2  命令会将test整个文件夹放到 /root/test2 文件夹下, 
但是 ADD命令是将 ./test文件夹下面的所有东西 放到/root/test2文件夹下 
相当于 ```cp -r ./test/* /root/tes2```

#### 3.1.6 Dockerfile常见命令解析
|  命令  |  描述  |  示例  |   注意事项  |
|  ---- | ------ | ------ | ---------- |
|   FROM     |    指定基础镜像   |    FROM <镜像>:[TAG]     |     无    |
| MAINTAINER |    镜像的维护者   | MAINTAINER 'eugenehuang@summary.com.cn' |    无     |
|   COPY     | 将宿主机的文件复制到镜像中去 | COPY  源文件(夹) 目标文件(夹)  |     注意: 源文件路径必须与build同级,不能是其父级  |
|   ADD      | 将宿主机的文件添加到镜像中去 |  ADD 源文件(夹) 目标文件(夹)   |     注意: 源文件路径必须与build同级,不能是其父级  |
|  WORKDIR   | 指定工作目录, 在该命令下执行的文件操作 | WORKDIR /usr/local/src |  若在此命令后面执行了ADD或COPY命令,那么目标文件(夹)都会添加/usr/local/src前缀|
|     ENV    |   指定环境变量, ENV <key>=<value> 或 ENV key value |  ENV JAVA_HOME /usr/local/jdk 、 ENV PATH $PATH:$JAVA_HOME/bin/ | 无 |
|    RUN     |   后面接shell脚本的命令, 会按照shell脚本的格式解析  |   RUN echo 'Hello docker'  |  无
|    CMD     |   后面接shell脚本命令, 与RUN不同的是, 该CMD后面接的命令是在docker中执行的 | 无 | 无
#### 3.1.7 指定docker 容器的时间参照物
* 背景: 在前后端分离的项目中, 难以避免在前端使用new Date()函数, 该函数获取的是当前电脑的时间, 
        加入当前电脑是UTC标准时间, 那么就会比我们正常的中国时间少8个小时。  
        所以, 根据这种情况, 会衍生出一种case: 就是在本地显示的时间是好的, 但是一上docker化的  
        dev或者qa或者生产环境的时候就会出现少了8个小时, 原因是dev、qa、生产环境是将nginx服务  
        器放在docker里, 会根据docker的时间区来获取时间戳的年月日, 进而出现本地环境和dev、qa、  
        生产环境出现不一样的情况
* 解决方案: (设置容器中的时间与当地的保持一致即可)
        在制作docker的Dockerfile文件添加如下配置:
          ENV TZ=Asia/Shanghai
          RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo '$TZ' > /etc/timezone


### 3.2 Jenkins
#### 3.2.1 自动化部署maven项目
#### 3.2.2 多job部署, job间传值
#### 3.2.3 linux不同用户运行jenkins.war
```
linux若分别以普通user启动jenkins.war, 那么会在/home/user/.jenkins/ 目录下建job目录.
若以root的身份启动的话, 则会在/root/.jenkins/ 目录下建job目录.
所以在后续需要启动jenkins时, 要注意使用root身份启动还是user身份启动, 因为他们读取的job目录是不一样的.
```
#### 3.2.4 Jenkins支持maven多模块项目(每个模块都是一个git仓库)多环境同时部署思想
* 背景:
```js
问: 什么情况下会不支持多环境同时部署?
答: 众所周知, maven项目的仓库设置的只有一个, 当在同一台搭建jenkins的电脑部署生产环境和测试环境的时,
    使用的是同一个本地仓库, 生产环境一般部署是master分支, 测试环境部署测试环境的branch, 在maven项目build
    的过程中, 一般都需要install jar包到本地仓库, 以便于打包的时候能找到依赖. 试问, 同时install不同branch的
    jar包, 但jar包的groupId、artifactId、version都没有改变, 那肯定会出问题呀.

解决方案:
  引入版本控制插件:
  1. 在根项目pom文件中的build -> plugins标签中添加如下代码, 引入插件:
    <plugin>
      <groupId>org.codehaus.mojo</groupId>
      <artifactId>versions-maven-plugin</artifactId>
      <version>2.3</version>
      <configuration>
        <generateBackupPoms>false</generateBackupPoms>
      </configuration>
    </plugin>
  2. 在每个环境中部署前执行命令
    mvn versions:set -DnewVersion=版本号
    该命令的含义是根项目的pom文件的version设置成上面的 "版本号"
    同时会将其它模块依赖另一个模块的version号都更新成上述的 "版本号"
    (Notice: 子模块不要添加自己的version, 要完全依赖父模块的version), 否则pom文件会乱.
  3. 每一个模块打包的版本都指定好了, 随后直接install & package就行了。
    注意: 最好是每一个环境都有一个对应的backend项目, 否则在部署qa环境的时候, 运行了更新版本号的命令, 
    并且在install的过程中, 又需要同时部署生产环境, 那么此时又会重新设置每一个模块的版本号。
    要解决这个问题则是每一个环境有一个对应的backend目录, 并对该banckend目录更新版本号进行打包
  4. 打包完成后, 还要修改对应的制作镜像的Dockerfile文件, 因为要指定具体的目录拿具体打包好的jar包
```
#### 3.2.5 jenkins multijob build多模块(每个模块都是一个git仓库)
* 背景: 在多模块的springboot项目中, 可能会存在项目中统一以来的common类库(自己编写的), 在改common类库
        会添加许多common的配置, eg: jdbc, log, mybatis mapping扫描包, mybatis别名配置等等. 所以
        在模块打包时, 需要保证common的类库已经存在与maven 本地仓库了, 此时multijob的作用就体现了出来.
* multijob: multijob是一个插件, 它可以控制jenkins job的执行顺序, 串行还是并行.
* 实现步骤:
    1. 建立一个Multijob pipeline(外层, 主要是一个壳子, 该途径可以让job之间串行或者并行) 参数化构建.  
       添加参数, 一般都是branch name, 这样就能指定拉去哪个环境的代码了
    2. 在ADD BUILD STEP TAB下添加一些阶段(phase)性的job, 可以设置串行或者并行
       串行即使用队列(sequence)的方式, 并将触发机制设置成successful
       并行则使用并列(parallel)的方式, 并将触发机制设置成always
       即在这可以设置一些job的执行顺序, 这样就可以解决一些项目依赖与另一个项目先启动的问题,
       eg: 要先启动eureka再启动其他服务, 因为其他服务要往eureka注册
#### 3.2.6 jenkins Multijob 参数传递规则:
1. 通过build step为downstream job phase的传递规则, downstream job 参数名必须与upstream  
   job定义的参数名一致, 这样在upstream job的multijob触发downstream job phase时,  
   downstream job才能接收到参数.
2. 通过post-build-action为trigger parameterized build on other projects的传递规则  
   通过设置parameters type为predefined paremters的方式, 以key=value的方式定义传递参数,  
   ps: 要获取upstream job传递的参数或者当前job自定义的参数时要使用${key}的方式

#### 3.2.7 jenkins使用nohup后台运行jar包
* 背景  
    在linux环境中启动一个程序想放入后台正常做法是使用nohup加&符号。 

* 解决方案  
    需要使用如下命令: 
      nohup java -jar xxx.jar > myLog.log 2>&1 &
    将日志输出重定向到myLog.log文件中

#### 3.2.8 jenkins运行mvn命令找不到
* 背景:  
  ```
    在安装maven时, 配置环境变量配置到了~/.bashrc(~/.bash_profile)文件, 该文件的环境变量是针对于当前用户而言,
    导致在jenkin build maven项目时提示命令找不到, 因为jenkins运行命令时, 他所处的用户组和用户是
  ```
* 

### 3.3 Shell脚本
#### 3.3.1 自定义shell脚本, 完成maven多项目自动拉取远程仓库代码操作
#### 3.3.2 ENV=${ENV:-"local"} 代码含义
* 首先这是一个定义变量的过程, ${}里面的ENV是变量名接收值, 相当于springboot的@requestParam(value = 'a', defaultValue="string") String b 中的a, 用来接收参数,而后面的local是默认值, ```中间一定要加横线```所以在执行脚本时设置参数值是这样表示的:  ENV=test ./脚本名字那么此时脚本中的ENV变量就会变成test
#### 3.3.3 ssh执行远程命令awk命令无法执行的问题
* 使用双引号将整个命令包括起来, 使用单引号将awk后面的表达式括起来, 并在$x前添加转义符(\)
  eg: ssh -i xxxx.pem root@100.20.33.190 "docker ps -a | grep vue-docker-v1 | awk '{print \$1}'"
  命令解析: 将docker信息包含vue-docker-v1的容器输出第一个参数(containerId), 
           这么做的原因通常是在部署时, 需要停止容器再重新打镜像.
#### 3.3.4 Sed命令根据key修改文件内容
* sed -i "s/需要修改的key/需要修改的内容/g" 目标文件
  (后面加了一个g表示全局替换, 与正则中的g含义一致)
#### 3.3.4 Sed和Rename命令修改文件名
* eg: 将test111.txt文件名中的1全部替换成2
  ```shell
    echo test111.txt | sed "s/1/2/g" | xargs mv test111.txt
  ```
* 替换文件名的命令还有rename命令, 但是该命令是批量修改文件名
  eg: 将当前目录下的所有htm后缀的文件统一改成html后缀
    ```shell
      rename "s/\.htm/\.html" *.htm
    ```

### 3.4 Nginx
#### 3.4.1 配置反向代理
* 在server部分添加如下配置:
```ngxin
  location /api/ {
    proxy_pass http://127.0.0.1:8001/;
    proxy_set_header Host $host;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header REMOTE-HOST $remote_addr;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
  }

表示: 当遇到后缀到/api的路由时, 反向代理到 127.0.0.1:8001,

反响代理允许重新定义或者添加http请求头
语法: proxy_set_header field value;
```
#### 3.4.2 配置多个vue.js单页面项目
*  在server部分添加如下配置:
```shell
location / {
  try_files $uri $uri/ /index.html;
}

if (!-e $request_filename) {
  rewrite ^/expo/.* /expo/index.html last;
}

----------------------------------------------
含义: 
  第一个配置为常见的vue.js单页面配置, 只需要添加这行配置, 并将打好的包放入ngxin访问的根目录下即可完成部署

  第二个配置为配置多个vue.js单页面的配置:
  解析:
    条件: 若请求的资源不是一个文件
    条件内语句块: 若请求uri中以expo为前缀, 则重定向到 uri为/expo/index.html

    注: 1. 要保证build后的所有文件放在ngxin根目录下的expo文件夹下.
        1. 静态资源要以expo文件夹为基准
```
eg: 在vue脚手架3.0版本之前, 初始化项目并采用[默认build的方式](https://github.com/EugeneHuang9638/treadpit/blob/master/common-build.png)打包的index.html文件内容为
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset=utf-8>
    <meta name=viewport content="width=device-width,initial-scale=1">
    <title>expo</title>
    <link href=/static/css/app.2f09759cd2fab12147a7ee7a21efe173.css rel=stylesheet>
  </head>
  <body>
    <div id=app></div>
    <script type=text/javascript src=/static/js/manifest.28e76dc415eb565ab385.js></script>
    <script type=text/javascript src=/static/js/vendor.3af6701d2adeecbcec08.js></script>
    <script type=text/javascript src=/static/js/app.04c768f7c6f8cd515016.js></script>
  </body>
</html>
```
   重点在于link标签的```script```标签, 默认为当前目录下的static文件夹下. 其实真正的规则为
   ```${assetsPublicPath}/${assetsSubDirectory}/css(js)/xxxx.css(js)```
   而```assetsPublicPath```和```assetsSubDirectory```变量可以在```config/index.js```[文件中](https://github.com/EugeneHuang9638/treadpit/blob/master/common-build.png)配置,
   所以在上述的配置中, 若请求的url为: ```127.0.0.1/expo/test``` 那么nginx内部会重定向到 ```127.0.0.1/expo/index.html``` 即进入ngxin第二种路由: 此时index.html各种静态资源在ngxin可访问的根目录下, 此时会报404.
   
   如果要访问expo/index.html 文件访问成功
   1. 首先在ngxin根目录下创建```expo```文件夹
   2. 并修改vue.js配置文件即build后的index.html文件  如下图:
      ![修改后的配置文件](https://github.com/EugeneHuang9638/treadpit/blob/master/modified-build.png), 
      ![修改配置后的index.html文件](https://github.com/EugeneHuang9638/treadpit/blob/master/modified-index.html.png)
   3. 将build后的包整个丢进expo文件夹内
   4. 重新reload ngxin, 再次访问即可

#### 3.4.3 docker化basic auth(可配)
1. 拉取准备好的镜像包
  ```
    git clone https://github.com/EugeneHuang9638/docker-nginx-basic-auth.git
  ```
2. 执行命令
  ```
    TAG=auth USERNAME=eug PASSWORD=pwd123 ./build.sh docker_build
  ```

各细节可跟踪至该[repository](https://github.com/EugeneHuang9638/docker-nginx-basic-auth.git)

#### 3.4.4 配置Https证书, 支持https访问.

***

## 四. Linux
### 4.1 常用命令(常忘)
#### 4.1.1 给文件添加可执行权限
* eg: chmod +x build.sh
#### 4.1.2 删除当前文件夹内所有内容
* rm -r *
#### 4.1.3 压缩当前文件夹为zip包
* zip -r target.zip ./
#### 4.1.4 解压缩zip压缩包到当前目录
* unzip target.zip -d ./  或  unzip target.zip
#### 4.1.5 查看某个文件的大小
* du -h 文件名
#### 4.1.6 列出文件夹下面第一级每个文件的大小(包括文件夹和文件)
* du -ah --max-depth=1 文件夹名
#### 4.1.7 查找文件命令
* 基本: find / -name '文件名
* 通配符: find / -name '*.conf*'
#### 4.1.8 查找某个端口被占用
* ps -ef | grep 80
* netstat  -anp | grep 80
#### 4.1.9 查看linux各进程内存使用情况
* top
* 指定某个线程: top | grep 进程名
#### 4.1.10 Linux 启动项目后台保留策略
* 背景: 通常要在后台执行会加上 & 符号, 但这样不稳定, 也许你关闭终端后, 通过这样的方式运行的程序就会挂掉.
* 目的: 要想脱离终端来执行程序的话应该使用 nohup命令, 三要素(nohup 运行的命令  & )
* 示例: 示例是运行一个打包好的springboot项目(后台启动项目, 并使用dev环境的配置)  
        nohup java -jar test.jar --spring.profiles.active=dev --server.port=8888 & 
#### 4.1.11 cp -r 命令的坑
```shell
在执行 cp -r 源文件夹  目标文件夹命令时,
若目标文件夹中存在一个与源文件夹同名的文件夹的话, 那么它会将整个源文件夹copy到目标文件夹中同名文件夹的里面
eg: cp -r /root/test /root/info/test  => 它会将/root/test copy到/root/info/test下, 
    所以/root/info/test 里面会多一个test文件夹. 

ps: 它并不是将/root/test文件夹中的内容copy到/root/info/test中, 若要实现此需求, 请执行
    cp -r /root/test/* /root/info/test
```
#### 4.1.12 清除所有log文件(内存不够时)
* find . -name "*.log | xargs rm"

#### 4.1.13 压缩成tar.gz压缩包
* 将当前目录压缩成test.tar.gz
  ```shell
    tar -czf test.tar.gz ./*
  ```

#### 4.1.14 解压缩tar.gz包
* 解压缩test.tar.gz包 至root目录下
  ```shell
    tar -zxvf test.tar.gz -c /root
  ``

#### 4.1.15 Linux文件权限查看及无权限解决方案
* 如下图
![文件权限解读图](https://github.com/EugeneHuang9638/treadpit/blob/master/linux_file_permission.jpg)

## 五. Http
### 5.1 ContentType
* ContentType存在的意义:
  在互联网中有成百上千种不同的数据类型, 它用来定义数据类型的格式.
* 在请求头中指定ContentType的意义:
  告诉服务器使用什么格式以及编码来解析请求中的消息
  eg: Content-Type: application/json;charset:utf-8;
* 常用的ContentType类型:
  ```
    1. application/x-www-form-urlencoded
       这种类型是将请求参数url编码后, 放到请求体中, 通常用于表单的提交. 通常会在后面添加 ;charset:utf-8 保证中文不乱码  
    2. application/json
       使用这个类型，需要参数本身就是json格式的数据，参数会被直接放到请求实体里，不进行任何处理。服务端/客户端会按json格  
       式解析数据（约定好的情况下）get请求下会将key-value解析出来，放到URL的参数里面
  ```

## 六. IDEA
### 6.1 快捷键
#### 6.1.1 查看接口或接口中的方法实现类
* Ctrl + Alt + b

## 七. 阿里云oss
### 7.1 上传图片
#### 7.1.1 私密上传base64格式图片
```java
  OSSClient ossClient = new OSSClient(endpoint, accessId, accessKey);
  ObjectMetadata objectMetadata = new ObjectMetadata();

  // 此段代码设置是否为私密
  objectMetadata.setObjectAcl(CannedAccessControlList.Private);
  ossClient.putObject(bucket, fileName, new ByteArrayInputStream(Base64.getDecoder().decode(imgBase64)), objectMetadata);

```
### 7.2 下载图片
#### 7.2.1 前端访问私密图片
* 原理: 根据需要请求的资源, 由后端对此资源进行临时授权(新增签名以及请求过期时间, 返回对该资源访问的完整url), 具体参考[oss临时授权文档, ```使用签名URL进行临时授权部分```](https://help.aliyun.com/document_detail/32016.html?spm=a2c4g.11186623.2.13.4de27e31juVYXF)


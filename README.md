# SpringMVC-01
简单使用

### 第一步
引入相关包(如使用maven，可以在编码过程中被动引入，可忽略此步)


### 第二部
配置web.xml
添加spring的核心servlet:**DispatcherServlet**  <br/>
并为servlet设置配置参数文件 <br/>
配置参数为<context:component-scan base-package="com.wby" />

### 第三部
编写C（控制器）模块 <br/>
设置监听地址及返回（模型）或（视图）模块 <br/>

编写M(模型）模块 <br/>
编写被c调用而进行逻辑处理，返回相关参数，来映射视图模块 <br/>

编写v(视图)模块 <br/>
进行JSP及Html文件的编写


## 相关知识点
注解类 <br/>
注解简化代码并提高编码的效率 <br/>
Java反射来处理注解 <br/>
spring四大注解类：Component，Controller,Service,Repository <br/>

### RequestMapping注解类


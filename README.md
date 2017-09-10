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

存在于Controller控制器类中 <br/>
1，使用@Controller注解标注控制类 <br/>
2，在配置文件中设置 <context:component-scan/> 对指定包进行扫描 <br/>
3，在控制类的类定义和方法定义上都可以标注@RequestMapping注解，分别对顶层和细节地址进行划分 <br/>
4,DispatcherServlet截获请求后，就通过@RequestMapping对请求进行映射处理方法 <br/>
#### RequestMapping 属性
value：    requestmapping 属性 指定请求的实际地址，指定的地址可以是URI Template 模式； <br/>
method：  指定请求的method类型， GET、POST、PUT、DELETE等,默认为GET； <br/>
consumes： 指定处理请求的提交内容类型（Content-Type），例如application/json, text/html；<br/>
produces:   指定返回的内容类型，仅当request请求头中的(Accept)类型中包含该指定类型才返回； <br/>
params： 指定request中必须包含某些参数值是，才让该方法处理. <br/>
headers： 指定request中必须包含某些指定的header值，才能让该方法处理请求。 <br/>

地址的正则：
\* <br/>
** <br/>
？？ <br/>
{userid} <br>

##### @PathVariable
可以将 URL 中占位符参数绑定到控制器处理方法的入参中：URL 中的 {xxx} 占位符可以通过@PathVariable("xxx") 绑定到操作方法的入参中。<br/>
##### @RequestParam 属性 value，required,defaultValue
相当于request.getParameter("name"); <br/>

##### @CookieValue 属性 value，required,defaultValue
与上面类似
。。。





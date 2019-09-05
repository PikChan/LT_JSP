# LT_JSP
学习JSP的旅程

## 一、概述：

本仓储库用来记录JSP的学习之旅。

指导思想：于建国的学习观，用例子来学习理论与概念而不是反之。

### 1.1 JSP的不足

>   但是，让页面美术设计师和开发人员在同一文件上工作并不理想，让Java嵌入HTML被证明是就象将HTML 嵌入Java一样令人尴尬。读取一堆很乱的代码仍然是一件困难的事情。   

>   于是，人们在使用jsp方面变得成熟，更多地使用了JavaBeans。 Beans包含了jsp所需的业务逻缉代码。JSP中的大多数代码都可以**取出来放到bean中去**，而只留下极少的标记用于调用bean。

!! https://wenku.baidu.com/view/f1943b42a8956bec0975e36b.html?from=related!

  ### 1.1.1EL的不足
        
   通过上面的例子，使用EL函数似乎和自定义标签一样，可以移除JSP中出现的Java代码，但是EL函数比自定义标签的不足之处在于，EL函数只能移除与web无关的方法，无法移除与web有关的方法，比如某些方法中含有 HttpServletRequest、HttpServletResponse等等这样的对象，因为在定义静态方法的时候，我们无法使用到这些web对象，这些web对象都是由Tomcat服务器返回这些接口的实例对象的，这都是服务器中低层封装好的，我们平常使用静态方法根本无法获取，因此此时还是需要使用自定义标签的

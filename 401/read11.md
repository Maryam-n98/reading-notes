
# Read: 11 - Spring

### Spring App Basics:

A Spring MVC is a Java framework which is used to build web applications. It follows the Model-View-Controller design pattern. It implements all the basic features of a core spring framework like Inversion of Control, Dependency Injection.

A Spring MVC provides an elegant solution to use MVC in spring framework by the help of DispatcherServlet. Here, DispatcherServlet is a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.

###### Spring Web Model-View-Controller

- Model - A model contains the data of the application. A data can be a single object or a collection of objects.
- Controller - A controller contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.
- View - A view represents the provided information in a particular format. Generally, JSP+JSTL is used to create a view page. Although spring also supports other view technologies such as Apache Velocity, Thymeleaf and FreeMarker.
- Front Controller - In Spring Web MVC, the DispatcherServlet class works as the front controller. It is responsible to manage the flow of the Spring MVC application.

## Thymeleaf

- Thymeleaf is a popular server-side template engine for Java applications. You can easily integrate it into a Spring Boot project to develop web applications.

 - In a standard Spring MVC application, the controller classes are the ones that collect data from different sources like databases or RESTful APIs, and then select a view to render and return the HTML back to the user. They create a model map with data that is later converted into a Thymeleaf context object.

##### Spring Model Attributes
Spring model attributes are useful for transferring data from Spring controllers to Thymeleaf views. In Thymeleaf terminology, they are called context variables.

- There are several ways to add model attributes to a view in Spring MVC. The simplest way is to use the Model's addAttribute()

**Accessing the attributes depends upon where they were added. If the attributes were added to the ModelAndView object, they must be accessed throught "${modelAndView.model.xxxx}" where xxxx is the attribute name. If the attributes were added to Model object, they are accessible using just the attribute name itself "${attributeName}".**


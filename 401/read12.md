
# Read: 12 - Spring RESTful Routing & Static Files

## Baeldung: Spring Request Mapping

**Request Mapping Basics**
In Spring MVC applications, the RequestDispatcher (Front Controller Below) servlet is responsible for routing incoming HTTP requests to handler methods of controllers.

When configuring Spring MVC, you need to specify the mappings between the requests and handler methods.

**@RequestMapping With @RequestParam**
The @RequestParam annotation is used with @RequestMapping to bind a web request parameter to the parameter of the handler method.

The @RequestParam annotation can be used with or without a value. The value specifies the request param that needs to be mapped to the handler method parameter, as shown in this code snippet.

**@RequestMapping Consumes and Produces**
Mapping media types produced by a controller method is worth special attention.

We can map a request based on its Accept header via the @RequestMapping headers attribute introduced above:
`
@RequestMapping(
  value = "/ex/foos", 
  method = GET, 
  headers = "Accept=application/json")
@ResponseBody
public String getFoosAsJsonFromBrowser() {
    return "Get some Foos with Header Old";
} `

**http://localhost:8080/spring-rest/ex/foos**

**Using @RequestMapping With HTTP Methods**

The Spring MVC @RequestMapping annotation is capable of handling HTTP request methods, such as GET, PUT, POST, DELETE, and PATCH.

By default, all requests are assumed to be of HTTP GET type.

In order to define a request mapping with a specific HTTP method, you need to declare the HTTP method in@RequestMapping using the method element as follows.

**RequestMapping With Path Variables**
Parts of the mapping URI can be bound to variables via the @PathVariable annotation.

**New Request Mapping Shortcuts**

@GetMapping
@PostMapping
@PutMapping
@DeleteMapping
@PatchMapping


## Accessing Data with JPA
**JPA**
 (Java Persistence API):
  JPA is a specification. It is a collection of classes and methods to persistently store the vast amounts of data into a database. It provides common prototype and functionality to ORM tools. By implementing the same specifiation, all ORM tools (like Hibernate, TopLink..) follows the common standarts.


**CrudRepository, JpaRepository, and PagingAndSortingRepository in Spring Data :**
Notice the typical CRUD functionality:

- save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
- findOne(…) – get a single entity based on passed primary key value
- findAll() – get an Iterable of all available entities in database
- count() – return the count of total entities in a table
- delete(…) – delete an entity based on the passed object
- exists(…) – verify if an entity exists based on the passed primary key value


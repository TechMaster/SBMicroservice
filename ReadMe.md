# Khoá học Spring Boot Microservice cho công ty Hyperlogy

[Outline thiết kế ban đầu](SpringBootMicroservice.pdf)

## Triển khai Spring Boot REST API
- Cấu trúc thư mục dự án Spring Boot
- Multilayer Architecture: View - Controller - Service - Repository
- Model View Controller
- Annotations: @Controller, @RestController, @Service, @Repository
- @PathVariable vs @PathParameter
- @RequestBody
- @RequestMapping, @GetMapping, @PostMapping, @PutMapping, @DeleteMapping
- So sánh giữa Server Side Render vs Client Side Render
- @CORS dự án Vue.js kết nối 

## Java Collection - Java Stream API
So sánh công dụng, trường hợp sử dụng
- List: ArrayList, Vector
- Set: HashSet, LinkedHashSet, TreeSet
- Map: HashMap, LinkedHashMap, TreeMap
- [4 cách iterate collection](https://www.codejava.net/java-core/collections/the-4-methods-for-iterating-collections-in-java)
- Java Stream API: stream, collect, groupby, filter, compare

Bài tập:
- Web site phân tích dữ liệu People Data 1000 bản ghi
Tham khảo:
- [Java Collections Framework API](https://www.codejava.net/java-core/collections/overview-of-java-collections-framework-api-uml-**diagram**)
- [18 Java Collections and Generics Best Practices](https://www.codejava.net/java-core/collections/18-java-collections-and-generics-best-practices)


## Chữa bài tập phân tích dữ liệu bằng Java Stream


## Dependency Injection
- Application Context
- Component Scanning
- Component vs Bean
- @Autowired, @Configuration, @Bean, @Order, @Qualifier, @Lazy, @Prototype
- 3 phương pháp DI:
  - Constructor Injection (khuyến cáo)
  - Setter Injection
  - Field Injection (dễ)



## SOLID Patterns By Example
- Single Responsibility Principle
- Open for Extension, Close for Modification Principle
- Liskov Substitution Principle
- Interface Segeration Principle
- Dependency Injection

## Design Patterns #1 : Creational Patterns
- Abstract Factory
- Builder
- Adapter
- Factory Method
- Prototype
- Singleton

## Design Patterns #2 : Structural Patterns
- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy

## Design Patterns #3 : Behavioral Patterns
- Chain of Responsibility
- Command
- Iterator
- Mediator
- Observer
- Memento
- State
- Template method
- Strategy
- Visitor

## Distributed Tracing

Tham khảo
- [Distributed Tracing with Spring Cloud Sleuth and Zipkin - AQAP Series](https://dev.to/brunodrugowick/distributed-tracing-with-spring-cloud-sleuth-and-zipkin-3moo)
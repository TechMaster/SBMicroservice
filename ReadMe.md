# Khoá học Spring Boot Microservice / Spring Cloud
Giảng viên:
- Trịnh Minh Cường, cuong@techmaster.vn, 0902209011
- Bạn nào tìm được page này, code ví dụ mẫu đẹp - dạy được một số buổi thì liên hệ với mình với thông tin mình ghi rõ ở trên nhé.

Mô tả khoá học:
- [Outline thiết kế ban đầu](SpringBootMicroservice.pdf)
- Ưu tiên cho dev Java tuy nhiên dev back end ngôn ngữ khác cũng có thể hiểu.
- Học trực tuyến một tuần hai buổi. Mỗi buổi 120 phút. Cứ 30 phút nghỉ giải lao 3 phút
- **Không giao bài tập lập trình**, vì học viên chủ động áp dụng kiến thức luôn vào dự án. Giảng viên cũng không còn thời gian để chấm bài tập.
- Một số chủ đề khó, giảng viên chỉ dạy 1 tuần 1 buổi.
- Sau buổi học thứ 12: học viên không hài lòng nội dung kiến thức, sư phạm của giảng viên hoặc cảm thấy tự học được -> Dừng lớp học. Mình có nhiều dự án không kịp xử lý.
- Đây là một khoá học rút ngắn thời gian, công sức tự học, mày mò của học viên. Code minh hoạ dễ hiểu, trực quan, không phải code nào cũng có chất lượng production ready.

## 01: Triển khai Spring Boot REST API
- Cấu trúc thư mục dự án Spring Boot
- Multilayer Architecture: View - Controller - Service - Repository
- Model View Controller
- Annotations: @Controller, @RestController, @Service, @Repository
- @PathVariable vs @PathParameter
- @RequestBody
- @RequestMapping, @GetMapping, @PostMapping, @PutMapping, @DeleteMapping
- So sánh giữa Server Side Render vs Client Side Render
- @CORS dự án Vue.js kết nối 

## 02: Java Collection - Java Stream API
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

## 03: Lombok. Try Catch Exception - Logging
- Lombok
  - @Data, @NoArgConstructor, @AllArgsConstructor, @Builder
- Check vs Uncheck Exception
- Custom Exception
- Log4J2:
  - Lombok @SLF4J
  - Cấu hình Logging
  - Logging to file, console
  - Điều hướng từng dòng log theo Exception
  
## 04: Dependency Injection
- Application Context
- Component Scanning
- Component vs Bean
- @Autowired, @Configuration, @Bean, @Order, @Qualifier, @Lazy, @Prototype
- 3 phương pháp DI:
  - Constructor Injection (khuyến cáo)
  - Setter Injection
  - Field Injection (dễ)

## 05: JUnit5 - AssertJ
- Các annotation @BeforeAll, @AfterAll, @BeforeEach, @AfterEach, @Test
- Điều kiện chạy test case
- Sử dụng AssertJ nối chuỗi các biểu thức kiểm tra. Fluent API

## 06: JPA #1 định nghĩa Entity
- Data Access Object pattern
- @Table: chú ý tránh các keyword trong SQL, snake_case
- @Entity
- @Id, @AutoGeneratedValue, Auto vs Identity
- @Column: name, unique, nullable, insertable, updatable, length, columnDefinition
- @NaturalId
- @Transient
- @Temporal
- @Enumerated
- @Embedded  - @Embeddable
- @Index : single colulm - multiple columns
- @PrePersit - @PreUpdate - @PreRemove

## 07: JPA #2: Relationships in JPA
- One : One
- One : Many -> Unidirection vs Bidirectional
- Many : Many -> không cột trung gian vs có cột trung gian, sử dụng primary riêng vs sử dụng composite primary key
- Cascade Operation: orphanRemoval
- @LazyLoad, EagerFetch
- JSON serializeserialize: @JsonIgnore, @JsonGetter, @JsonManageReference, @JsonBackReference
- Inheritance: Mapped Class, Single Table, One Table per Class, Joined Table, Polymorphism Query
- Entity Manager
- Testing Entity Manager
  
## 08: JPA #3:Repository & Query.  Transaction và Nested Transaction
- Repository khác biệt gì với EntityManager
- Custom Repository
- Viết Derived Query với cú pháp JPQL: WHERE, LIKE, JOIN, GROUP BY
- Nested Transaction
- Transaction Context
- Commit / Rollback on Exceptions

## 09: SOLID Patterns By Example
- Single Responsibility Principle
- Open for Extension, Close for Modification Principle
- Liskov Substitution Principle
- Interface Segeration Principle
- Dependency Injection Principle (đã nói ở phần trước rồi)
- Sẽ trình bày luôn AspectJ

## 10: Aspect Programming áp dụng cho Spring Boot
- Aspect
- Join Point
- Advice
- Point Cut
- Introduction
- Target Object
- AOP Proxy
- Weaving

## 11: REST nâng cao #1
- Hibernate Validation: @Size, @NotBlank, @Email, @Pattern + Regex
- DTO: Data Transfer Object
- Object Mapping với MapStruct

## 12: REST nâng cao #2
- Custom Exception Handling
- Open API / Swagger

## 13: REST nâng cao #3
- Open Feign Client kết nối REST API
  - import package
  - define Open Feign Interface
- Spring Retry khi kết nối không thành công

## 14: Bên trong Spring Boot application
- Spring Boot Event
  - publish event
  - ApplicationListener
  - @EventListener
  - @EnableAsync  
- Scheduling
  - @Scheduled, @EnableScheduling
  - Fixed Delay vs Fixed Rate
  - Intial Delay
  - Khai báo Cron Job 
- Spring Boot Actuator


## 15: Design Patterns #1 : Creational Patterns
- Abstract Factory
- Builder
- Adapter
- Factory Method
- Prototype
- Singleton

## 16: Design Patterns #2 : Structural Patterns
- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy

## 17: Design Patterns #3 : Behavioral Patterns
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


## 18: Spring Security #1
- @EnableWebSecurity
- @EnableGlobalMethodSecurity
- UserDetailService: InMemoryDetailService, CustomDetailService
- PasswordEncoder
- Role vs Authority
- AntMatchers

## 19: Spring Security #2: Expression Based Access Control + JWT
- Spring Expression Language
- @PreAuthorize vs @PostAuthorize
- @PreFilter vs @PostFilter
- JWT Authentication

## 20: OAuth2 + KeyCloak
- Cài đặt KeyCloak bằng Docker
- Cấu hình KeyCloak: Realm, Role, User
- OAuth2

## 21: Microservice Patterns
- Tóm tắt các Microservice Patterns
- Spring Cloud có những gì?
- Spring Cloud API Gateway
- Rate Limiter

## 22: Eureka Service Discovery - Centralized Configuration
- Spring Cloud Eureka
- Spring Cloud Config

## 23: Distributed Tracing
- Spring Cloud Sleuth
- [Distributed Tracing with Spring Cloud Sleuth and Zipkin - AQAP Series](https://dev.to/brunodrugowick/distributed-tracing-with-spring-cloud-sleuth-and-zipkin-3moo)

## 24: SAGA Patterns
- Distributed Commit and Rollback
- Kafka Publish / Subcribe Topic
  
## 25: Event Sourcing - CQRS
- Bản chất Event Sourcing
- Thiết kế triển khai Event Sourcing
- Giới thiệu CQRS (một buổi sợ không đủ)
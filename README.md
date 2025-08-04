# Bookstore-Microservice-Java

**The Problem**
 - Monolithic architecture limitations: Traditional bookstore applications were built as monoliths, leading to scalability and deployment issues as user base and feature set expanded.
 - Lack of centralized observability and fault tolerance: Without proper service discovery, logging, or circuit breakers, failures in one component could cause cascading issues across the entire system.

**The Hypothesis**
 - Microservices can improve modularity and scalability: By separating the bookstore application into independent services (User, Inventory, Cart), each can be scaled, deployed, and maintained independently.
 - Leveraging modern tools (Spring Cloud, Docker, RabbitMQ) will enhance system reliability and observability, reducing downtime and improving debugging.

**The Approach**
 - Adopted Spring Boot 3 and Java 17, applying domain-driven microservices design with services like User, Inventory, and Cart, managed under an API Gateway.
 - Integrated distributed system components: Used Eureka for service discovery, RabbitMQ for async communication, Zipkin and Micrometer/OpenTelemetry for tracing, and Docker Compose for consistent environment setup.

**The Outcomes**
 - Modular & Scalable Architecture: Each microservice is independently deployable and communicates through REST or RabbitMQ, reducing interdependency bottlenecks.
 - Improved reliability and observability: Failures were isolated using Resilience4j (circuit breaker), and developers could trace request flow using Zipkin, significantly improving debugging speed.

**Conclusion**
 - The microservice approach validated the hypothesis by improving deployment flexibility, development speed, and fault tolerance.
 - The project serves as a strong template for scalable, cloud-ready systems using modern Java and Spring tools, and offers extensibility for real-world production scenarios.

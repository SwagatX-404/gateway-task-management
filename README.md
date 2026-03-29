## GATEWAY FOR TASK MANAGEMENT SERVICE

## Database Configuration 
- [application.yaml] file
```bash 

server:
    port: 5000

spring:
  application:
    name: GATEWAY-SERVICE
cloud:
  gateway:
    mvc:
      routes:


default-filters:
        - DedupeResponseHeader=Access-Control-Allow-Credentials, Access-Control-Allow-Origin
      globalcors:
        cors-Configurations:
          '[/**]':
            allowedOrigins: "*"
            allowedMethods:
              - GET
              - POST
              - PUT
              - PATCH
              - DELETE
            allowedHeaders: "*"




eureka:
  instance:
    prefer-ip-address: true
  client:
    fetch-registry: true
    register-with-eureka: true
    service-url:
      defaultZone: http://localhost:8070/eureka/
```

## 👤 Author

**Swagat Murmu**  
*Master of Computer Applications (MCA)*
- **Primary Skills:** 
  - **Backend:** Java & Spring Boot
  - **Frontend:** React & JavaScript
  - **Database:** SQL

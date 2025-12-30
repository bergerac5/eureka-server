🧭 Eureka Server – Service Discovery Online Voting Microservices Architecture
==============================================================================
📌 Overview
------------
The Eureka Server is the Service Discovery Server for the Online Voting Microservice system.
It allows all microservices (API Gateway, Auth Service, Voter Service, Voting Service, etc.) to register themselves and discover each other dynamically without using hard-coded URLs.

This service is a core infrastructure component and must be running before any other microservice.
____________________________________________________________________________________________________________________________
🧱 Responsibilities
--------------------

Register microservices dynamically

Maintain service registry

Enable service-to-service discovery

Support client-side load balancing

Provide visibility into service health and availability
_______________________________________________________________________________________________________________________________________
🛠️ Tech Stack
--------------
Java 21

Spring Boot 3.1.8

Spring Cloud Netflix Eureka Server

Maven
**********************************************************************************************************
📂 Project Structure
---------------------
```
eureka-server/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/online/voting/eureka
│       │       └── EurekaServerApplication.java
│       └── resources/
│           └── application.yml
├── pom.xml
└── README.md

```
****************************************************************************************************************
🚀 Running the Service
-----------------------
Prerequisites
______________
Java 21

Maven
****************************************************************************************************************
🧩 Role in System Architecture
-------------------------------
```
               ┌──────────────────┐
               │  Eureka Server   │
               │  (Discovery)     │
               └─────────▲────────┘
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
 API Gateway       Auth Service     Business Services

```
--------------------------------------------------------------------------------------------------------------
👨‍💻 Author
----------

Irakarama Bergerac
Online Voting Microservice System

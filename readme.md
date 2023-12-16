# Currency Conversion Microservice

## Overview

The Currency Conversion Microservice is a Java-based microservice developed with Spring Boot and integrated with Spring Cloud components. It is designed to handle currency conversion operations and communicate with other microservices in a distributed system.

## Features

- **Currency Conversion:** Convert amounts between different currencies.
- **Microservice Architecture:** Built as a standalone microservice, allowing for independent development, deployment, and scalability.
- **Spring Cloud Integration:** Utilizes Spring Cloud components for service registration and discovery (Eureka) and declarative REST clients (Feign).

## Prerequisites

Before running the application, ensure you have the following installed:

- Java Development Kit (JDK)
- Integrated Development Environment (IDE) such as IntelliJ or Eclipse
- [Spring Boot](https://spring.io/projects/spring-boot)

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/currency-conversion-service.git


2. Open the project in your preferred IDE.

3. Review and update the application properties in src/main/resources/application.properties or src/main/resources/application.yml to match your environment.

4. Ensure that the necessary dependencies and plugins are configured in your Maven POM file.

# Configurations

## Application Properties

1. spring.application.name: Name of the microservice. (Default: currency-conversion)

2. server.port: Port on which the microservice will run. (Default: 8100)

3. spring.config.import: Configuration import strategy for connecting to a Config Server. (Optional: http://localhost:8888)

4. eureka.client.service-url.defaultZone: Eureka server URL for service registration and discovery. (Default: http://localhost:8761/eureka)


## Endpoints

- REST Template Endpoint: /currency-conversion/from/{from}/to/{to}/quantity/{quantity}

- Feign Client Endpoint: /currency-conversion-feign/from/{from}/to/{to}/quantity/{quantity}
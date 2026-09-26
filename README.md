# CloudMart — Platform

## Project Description

Parent repository grouping the three platform components of the CloudMart microservices capstone: the service registry, the config server and the API gateway. These run on two peer-aware GCE VMs (`platform-a`, `platform-b`) for high availability, giving the business services in [CloudMart-Services](https://github.com/vihanapathum/CloudMart-Services) service discovery, centralized configuration and a single public entry point.

| Submodule | Role | Port |
| --- | --- | --- |
| [cloudmart-service-registry](https://github.com/vihanapathum/cloudmart-service-registry) | Eureka service discovery | 8761 |
| [cloudmart-config-server](https://github.com/vihanapathum/cloudmart-config-server) | Spring Cloud Config Server | 8888 |
| [cloudmart-api-gateway](https://github.com/vihanapathum/cloudmart-api-gateway) | Spring Cloud Gateway, public entry point | 8080 |

## Technology Stack

- Java 25, Spring Boot 4.0.7, Spring Cloud 2025.1
- PM2 process management on GCE VMs

## Setup / Getting Started

This repo uses git submodules:

```bash
git clone --recurse-submodules https://github.com/vihanapathum/CloudMart-Platform.git
```

See each submodule's own README for build and run instructions.

## Student Information

- **Student Name:** A.G.Vihana Pathum Piyasiri
- **Student Number:** 2301692038
- **Slack Handle:** vihana_piyasiri
- **GCP Project ID:** project-1023ef7b-f75c-4e17-ab5

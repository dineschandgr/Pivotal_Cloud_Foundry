# Pivotal_Cloud_Foundry
Deploying Spring Boot Apps and Microservices to Pivotal Cloud Foundry


This Project has source code for multiple projects like

- Deploying a simple hello world application
- Application with H2 in-memory database
- Application with Mysql DB in local and also in the PCF as service
- Deploying full stack application with react and springboot
- Microservices with Eureka Service Discovery 
- Spring-cloud-config-server as API Gateway
- Spring Cloud Config server
- Deploying containers in PCF
- Auto scaling
- Circuit breaker using Hystrix

- Every application needs a unique route
- We need to have manifest.yml file with pcf config for every application
- react js and spring boot applications can have different manifest files or a combined manifest file
- Mysql, Eureka, Config Server, Hystrix etc are all configured as a service in PCF
- The services can be mentioned as a par tof manifest file

- manifest.yml file has the following config

1. application name
2. Memory
3. Route
4. Build pack
5. Services 
etc

- When an application is pushed using cf push, manifest file is used to determine the build pack
- With the source code and build pack, a droplet is created
- The droplet is then deployed into a container running inside the cell

PCF also provides

- Load balancing
- Auto scaling

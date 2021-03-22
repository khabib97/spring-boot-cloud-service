# spring-boot-cloud-service

Spring Boot Cloud Service has 3 sub-modules: 

1. Spring Microservice Client - limits-service
2. Spring Cloud Server - spring-cloud-config-server
3. Central Config Repo - config-repo-spring-cloud-service

>Ignore currency services

![Cloud Config Repo Model](https://static.javatpoint.com/tutorial/microservices/images/connect-Spring-cloud-config-server-to-local-git-repositorys.png)

- limits-service consumes configration data from cloud-config-server.
- cloud-config-server consume all configuration from centralized config-repo

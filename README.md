# spring-boot-cloud-service

Spring Boot Cloud Service has 3 sub-modules: 

1. Spring Microservice Client - limits-service
2. Spring Cloud Server - spring-cloud-config-server
3. Central Config Repo - config-repo-spring-cloud-service

>Ignore currency services

![Cloud Config Repo Model](https://static.javatpoint.com/tutorial/microservices/images/connect-Spring-cloud-config-server-to-local-git-repositorys.png)

- limits-service consumes configration data from cloud-config-server.
- cloud-config-server consume all configuration from centralized config-repo

# Project setup

- Download this repository 
```
git clone --recursive https://github.com/khabib97/spring-boot-cloud-service.git
```
- Make submodules to track their respective remote branches (instead of being in detached HEAD state):
```
git submodule foreach -q --recursive 'git checkout $(git config -f $toplevel/.gitmodules submodule.$name.branch || echo master)'
```
- Run `limits-service` and `spring-cloud-config-server` modules

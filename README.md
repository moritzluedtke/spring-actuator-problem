# spring-actuator-problem

This repo is showing a bug mentioned in https://github.com/spring-cloud/spring-cloud-commons/issues/788

## How to reproduce the error
1. Start the application like normal
1. Call `localhost:8001/ops/pause` -> Tomcat will shut down and the whole application stops.

With version `2.1.6.RELEASE` up until `2.2.8.RELEASE` of Spring Boot this was not an issue.

FROM openjdk:8-jre-alpine

MAINTAINER Hitham Ramzy <hitham.ramzy@gmail.com>

COPY eureka-service.jar eureka-service.jar

EXPOSE 8761

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar", "/eureka-service.jar"]
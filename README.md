# demo-spring-eureka-server
This demo is a eureka server to register applications in micro services.
This demo is using spring cloud and eureka server.

## Using Docker to simplify development

You can also fully dockerize your application and all the services that it depends on.
To achieve this, first build a docker image of, Please run:

    mvn package docker:build -X

Then run:

    docker-compose -f src/main/docker/app.yml up -d
    
## Close Docker container

To close docker container, Please run:
    
    docker-compose -f src/main/docker/app.yml down
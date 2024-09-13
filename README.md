# Microsservices Project Using Java Spring Boot And RabbitMQ
## An app divided into smaller portions for better scalibity and flexibility.

This is a project that was devoloped following along the course: Aprofunde em Java com arquitetura de Microsserviços, Spring e RabbitMQ from Alura.

  This is an app that deals with orders, payments and ratings. Each of which is its own service, that all run together with a eureka server, and gateway.
  The rabbitMQ instances are ran in Docker with the command 'docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.10-management' in the terminal.

## Running the project

1. Download the project
2. change environmental variables as deem necessary in applications-prod.properties
3. make sure to run the server, and gateway before running the other services, as they rely on them to work together

## Functions
* receive orders, payments and ratings from json requests
* services communicating with each other through rabbitMQ
* Assync responses to requests
* ability to run multiple instances of a single service

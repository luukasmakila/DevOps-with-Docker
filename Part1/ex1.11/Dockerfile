FROM openjdk:latest

EXPOSE 8080

COPY ./spring-example-project .

RUN ./mvnw package

ENTRYPOINT ["java", "-jar", "./target/docker-example-1.1.3.jar"]

FROM eclipse-temurin:17-jdk-alpine

RUN apk add --no-cache maven

ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

ENTRYPOINT ["java","-jar","app.jar"]

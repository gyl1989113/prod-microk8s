FROM openjdk:8-jdk-alpine
MAINTAINER HAOYANG 2019-02-18
WORKDIR /app
RUN mkdir config
COPY ijep-registry/ijep-registry-eureka/target/ijep-registry-eureka-6.0-SNAPSHOT.jar /app/ijep-registry-eureka-6.0-SNAPSHOT.jar
EXPOSE 9761
ENTRYPOINT ["java","-Xms100m","-Xmx100m","-jar","./ijep-registry-eureka-6.0-SNAPSHOT.jar","--spring.config.location=./config/application-eureka-beta.yml","--spring.profiles.active=eureka-beta"]


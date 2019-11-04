FROM openjdk:8-jdk-alpine
MAINTAINER HAOYANG 2019-02-18
WORKDIR /app/
RUN mkdir -p /app/config
COPY ./ijep-spider-service/target/ijep-spider-service.jar /app/ijep-spider-service.jar
EXPOSE 9300
ENTRYPOINT ["java","-Xms300m","-Xmx300m","-jar","./ijep-spider-service.jar","--spring.config.location=./config/application-spider-beta.yml","--spring.profiles.active=spider-beta"]

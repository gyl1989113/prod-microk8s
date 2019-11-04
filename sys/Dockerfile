FROM openjdk:8-jdk-alpine
MAINTAINER HAOYANG 2019-02-18
WORKDIR /app
RUN mkdir -p /app/config
COPY ijep-service/ijep-service-sys/target/ijep-service-sys.jar /app/ijep-service-sys.jar
EXPOSE 9101
ENTRYPOINT ["java","-Xms100m","-Xmx100m","-jar","./ijep-service-sys.jar","--spring.config.location=./config/application-sys-beta.yml","--spring.profiles.active=sys-beta"]

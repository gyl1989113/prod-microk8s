FROM openjdk:8-jdk-alpine
MAINTAINER HAOYANG 2019-02-18
WORKDIR /app/
RUN mkdir -p /app/config
ADD ./ijep-router/ijep-router-zuul/target/ijep-router-zuul.jar /app/ijep-router-zuul.jar
EXPOSE 8770
ENTRYPOINT ["java","-Xms200m","-Xmx200m","-jar","./ijep-router-zuul.jar","--spring.config.location=./config/application-zuul-beta.yml","--spring.profiles.active=zuul-beta"]

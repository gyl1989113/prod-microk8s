FROM openjdk:8-jdk-alpine
WORKDIR /app
RUN mkdir -p /app/config
#ADD application-oppo-beta.yml /root/oppo
COPY ijep-spy-oppo.jar /app/ijep-spy-oppo.jar
EXPOSE 9311
ENTRYPOINT ["java","-Xms300m","-Xmx300m","-jar","./ijep-spy-oppo.jar","--spring.config.location=./config/application-oppo-beta.yml","--spring.profiles.active=oppo-beta"]

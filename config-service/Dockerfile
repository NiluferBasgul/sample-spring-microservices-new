FROM openjdk:21-jdk-slim

WORKDIR /app

EXPOSE 8061

COPY target/config-service-1.1-SNAPSHOT.jar /app/config-service-1.1-SNAPSHOT.jar

ENTRYPOINT ["java", "-jar", "/app/config-service-1.1-SNAPSHOT.jar"]

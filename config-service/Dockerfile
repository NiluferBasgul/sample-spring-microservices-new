# Use the official OpenJDK image from DockerHub
FROM openjdk:21-jdk-slim

# Define the working directory
WORKDIR /app

# Expose the port your application will run on
EXPOSE 8061

# Copy the application JAR directly to the /app directory
COPY target/config-service-1.1-SNAPSHOT.jar /app/config-service-1.1-SNAPSHOT.jar

# Command to run the JAR file
ENTRYPOINT ["java", "-jar", "/app/config-service-1.1-SNAPSHOT.jar"]

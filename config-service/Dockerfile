# Use the official OpenJDK image from DockerHub
FROM openjdk:21-jdk-slim

# Define environment variables
ENV APP_FILE=config-service-1.1-SNAPSHOT.jar
ENV APP_HOME=/app

# Expose the application port
EXPOSE 8061

# Set the working directory to the app's directory
WORKDIR $APP_HOME

# Copy the application JAR and the startup script into the container
COPY target/${APP_FILE} $APP_HOME/
COPY run.sh $APP_HOME/

# Run the startup script, which will expand the environment variables and start the Java app
ENTRYPOINT ["sh", "/app/run.sh"]

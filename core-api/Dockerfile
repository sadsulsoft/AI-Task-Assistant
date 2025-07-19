# /core-api/Dockerfile

# Use a base image with Java installed
FROM openjdk:17-slim

# Set the working directory
WORKDIR /app

# Copy the compiled Java application (the .jar file) into the container
# You would replace 'your-app.jar' with the actual name of your built file
COPY target/your-app.jar app.jar

# Expose the port the application runs on
EXPOSE 8080

# Command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]

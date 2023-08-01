#FROM openjdk:17
#
#RUN mkdir -p /app
#
#ADD target/web-0.0.1-SNAPSHOT.war /app/web-0.0.1-SNAPSHOT.war
#
#EXPOSE 8080
#
#ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-cp", "/app/web-0.0.1-SNAPSHOT.war", "com.rungroop.web.WebApplication"]



# Use an official OpenJDK 17 image as the base image
FROM openjdk:17

# Set the working directory inside the container
WORKDIR /app

# Copy the packaged JAR file into the container
COPY web-0.0.1-SNAPSHOT.jar /app/web-0.0.1-SNAPSHOT.jar

# Expose the port that your Spring Boot app is running on
EXPOSE 8080

# Command to run your Spring Boot application
CMD ["java", "-jar", "web-0.0.1-SNAPSHOT.jar"]

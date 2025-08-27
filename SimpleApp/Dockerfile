# Use a lightweight JRE
FROM eclipse-temurin:17-jre-jammy

# Copy the jar file from target folder into the container
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} /app/app.jar

# Expose port 8080
EXPOSE 8080

# Run the app
ENTRYPOINT ["java","-jar","/app/app.jar"]

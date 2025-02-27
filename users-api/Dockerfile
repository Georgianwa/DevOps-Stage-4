FROM openjdk:17
WORKDIR /app
COPY target/users-api.jar users-api.jar
EXPOSE 8000
CMD ["java", "-jar", "users-api.jar"]
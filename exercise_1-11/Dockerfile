# Open Java Development Kit -> open source implementation of the Java Platform
FROM openjdk:8

EXPOSE 8080

WORKDIR /usr/src/app

# Copy everything to container
COPY . .

# Build the project
RUN ./mvnw package

# Run the project
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

# Build : docker build . -t spring-project
# Run : docker run -p 8080 spring-project

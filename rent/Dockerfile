FROM maven:3.8.6-jdk-11

WORKDIR /app
COPY . .
RUN mvn clean package
RUN cp ./target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "/app/app.jar"]
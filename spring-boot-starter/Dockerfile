FROM openjdk:8u181-jre-alpine

LABEL maintainer="KNFreightNet Graal Spacemission"
LABEL com.kn.department="Freightnet"
LABEL version="1.0"
LABEL com.kn.description="This is a KNFreightNet container for Spring Boot"

# The mock's jar file
ARG JAR_FILE=build/libs/spring-starter-demo-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} application.jar

ENTRYPOINT ["java", "-Xmx64m", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/application.jar"]

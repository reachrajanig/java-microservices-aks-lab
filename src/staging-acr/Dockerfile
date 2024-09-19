FROM mcr.microsoft.com/openjdk/jdk:21-ubuntu

ARG ARTIFACT_NAME
ARG APP_PORT

EXPOSE ${APP_PORT} 8778 9779

ARG JAR_FILE=${ARTIFACT_NAME}

ADD ${JAR_FILE} app.jar

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]


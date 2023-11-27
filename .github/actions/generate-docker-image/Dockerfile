FROM openjdk:17-jdk-slim-buster
ARG ARTIFACT_NAME

WORKDIR /application

COPY ${ARTIFACT_NAME} /application/artifact.jar

CMD ["java", "-jar", "artifact.jar", "--spring.profiles.active=docker"]
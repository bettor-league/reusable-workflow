FROM openjdk:17-jdk-slim-buster

RUN mkdir /application

COPY ${ARTIFACT_NAME} /application/artifact.jar

WORKDIR /application

EXPOSE ${EXPOSE_PORT}

CMD ["java", "-Xmx50m", "-jar", "/artifact.jar", "--spring.profiles.active=docker"]
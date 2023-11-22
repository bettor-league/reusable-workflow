FROM openjdk:17-jdk-slim-buster

RUN mkdir /app

COPY ${ARTIFACT_NAME} /app/artifact.jar

WORKDIR /app

EXPOSE ${EXPOSE_PORT}

CMD ["java", "-Xmx50m", "-jar", "/artifact.jar", "--spring.profiles.active=docker"]
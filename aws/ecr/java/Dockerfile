FROM openjdk:17-oracle

VOLUME /tmp
ADD path/to/compiled/app-1.0.jar app-1.0.jar
RUN sh -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.profiles.active=prod","-jar","/app.jar"]

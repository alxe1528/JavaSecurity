FROM openjdk:8-jre-alpine
MAINTAINER Dominik Schadow <dominikschadow@gmail.com>

VOLUME /tmp

ADD csrf-spring-security.jar app.jar

RUN sh -c 'touch /app.jar'

ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "app.jar"]
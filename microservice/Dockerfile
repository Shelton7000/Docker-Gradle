FROM frolvlad/alpine-oraclejdk8:slim
ENV MONGO_URL mongodb://localhost/microservice
EXPOSE 7000
RUN mkdir -p /microservice/
ADD build/libs/api-films-0.0.1-SNAPSHOT.jar /microservice/api-films.jar
ENTRYPOINT ["java", "-jar", "/microservice/api-films.jar"]
FROM maven:3.6.0-jdk-11-slim AS build
#WORKDIR ./nf_nwdaf/
COPY ./nf_nwdaf/src /home/app/src
COPY ./nf_nwdaf/pom.xml /home/app
RUN mvn -f /home/app/pom.xml clean package

EXPOSE 8080
#ENTRYPOINT ["java","-jar","/app.jar"]

#Start with a base image containing Java runtime
FROM openjdk:21-jdk-slim

#Information about who maintains the image
MAINTAINER gurpreet.cs.tsys@gmail.com

# Install curl and other dependencies
RUN apt-get update && apt-get install -y curl

#Add the application jar to the image
COPY build/libs/configserver-0.0.1-SNAPSHOT.jar configserver-0.0.1-SNAPSHOT.jar

#Run the application
ENTRYPOINT ["java","-jar","configserver-0.0.1-SNAPSHOT.jar"]




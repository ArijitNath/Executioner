#Base Image
FROM openjdk:8-jdk-alpine

#Port to expose
EXPOSE 8070

#Env varibale for Working Directory
ENV CACHE_APP_HOME /usr/src/app

#Locate and Create JAR path
ARG CACHE_APPLICATION_JAR=simplecache*.jar

#Copy jar to container app directory
COPY $CACHE_APPLICATION_JAR $CACHE_APP_HOME/simplecache.jar

#Set Working Directory
WORKDIR $CACHE_APP_HOME

#Start Command
ENTRYPOINT ["java","-jar","simplecache.jar"]

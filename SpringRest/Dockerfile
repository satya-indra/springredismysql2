# Start with a base image containing Java runtime
#FROM openjdk:8-jdk-alpine

FROM openjdk:8
ADD redis_demo-1-0.0.1-SNAPSHOT.jar springrestapi.jar
RUN bash -c 'touch /springrestapi.jar'

EXPOSE 8082

#ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-Dspring.profiles.active=$container" , "-jar",  "/carparkapi.jar"]

COPY wait-for-it.sh /wait-for-it.sh

RUN chmod +x /wait-for-it.sh

#ENTRYPOINT ["java", "-jar",  "/springrestapi.jar"]



# Add Maintainer Info

#RUN bash -c 'touch /app.jar'


# Make port 8080 available to the world outside this container

# The application's jar file
#ARG JAR_FILE=target/carpark2-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container

#ADD carpark2-0.0.1-SNAPSHOT.jar carpark.jar

#EXPOSE 8085

#CMD ["./wait-for-it.sh", "carparkdb:3306", "--", "java", "-jar", "carpark.jar"]

#CMD ["./wait-for-it.sh", "carparkdb:13306"]




# Run the jar file 
 
#ENTRYPOINT ["java", "-jar", "carpark.jar"]

#ENTRYPOINT ["java","-jar","/carpark.jar"]

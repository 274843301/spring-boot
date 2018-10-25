FROM docker.io/java:8
#VOLUME /tmp
#ARG JAR_FILE
#ADD ${JAR_FILE} mybatisplus_study1-0.0.1-SNAPSHOT.jar
#RUN bash -c 'touch /mybatisplus_study1-0.0.1-SNAPSHOT.jar'
#EXPOSE 9090
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/mybatisplus_study1-0.0.1-SNAPSHOT.jar"]
VOLUME /tmp
ADD mybatisplus_study1-1.0.jar app.jar
EXPOSE 9090
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

FROM java:8
MAINTAINER Eva Lopez Puente
EXPOSE 8080
VOLUME /tmp
ADD /target/Ejercicio3-4ServerMysql-0.0.1-SNAPSHOT.jar ServerMysql.jar
#ENV JAVA_OPTS=""
RUN bash -c 'touch /ServerMysql.jar'
ENTRYPOINT ["java","-Dspring.datasource.url=jdbc:mysql://localhost/ejercicio","-jar","/ServerMysql.jar"]

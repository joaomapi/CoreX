FROM java:8
VOLUME /tmp
ADD web_interface-0.0.1-SNAPSHOT.jar app.jar
WORKDIR / #forca que o RUN corra na root
RUN bash -c 'touch /app.jar'
EXPOSE 8080
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
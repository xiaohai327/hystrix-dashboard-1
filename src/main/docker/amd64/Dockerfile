FROM java:8
VOLUME /tmp
ADD hystrix-dashboard.jar app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Xmx64m", "-Xss256k", "-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

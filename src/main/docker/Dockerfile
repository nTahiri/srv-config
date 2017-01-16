#FROM netflixoss/java:8
FROM  ntahri/springboot-maven:3
VOLUME /tmp
ADD innolab-server-config-0.0.5.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]

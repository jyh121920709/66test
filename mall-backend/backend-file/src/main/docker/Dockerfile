#define basic image
FROM frolvlad/alpine-oraclejdk8
VOLUME /tmp
#add jar to docker
ADD backend-file-1.0-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
#after create ,operate
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
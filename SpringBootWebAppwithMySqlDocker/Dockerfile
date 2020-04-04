FROM openjdk:8
ADD target/app.jar app.jar
RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS="-Xdebug -Xrunjdwp:server=y,transport=dt_socket,address=8787,suspend=n"
#ENV SPRING_PROFILES_ACTIVE "default"
EXPOSE 8080
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -Dspring.profiles.active=$SPRING_PROFILES_ACTIVE -jar /app.jar" ]
ENTRYPOINT [ "sh", "-c", "java -jar /app.jar" ]

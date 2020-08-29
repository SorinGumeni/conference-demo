FROM openjdk:11-jre-slim
COPY target/conference-demo-0.0.1-SNAPSHOT.jar /app/app.jar
COPY docker/create_tables.sql /docker-entrypoint-initdb.d/
COPY docker/insert_data.sql /docker-entrypoint-initdb.d/
CMD ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app/app.jar"]

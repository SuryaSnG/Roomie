FROM openjdk:11

WORKDIR /app

COPY target/roomie.jar /app/roomie.jar

ENV SPRING_JPA_HIBERNATE_DDL_AUTO=update
ENV SPRING_DATASOURCE_URL=jdbc:mysql://localhost:3306/roomie
ENV SPRING_DATASOURCE_USERNAME=root
ENV SPRING_DATASOURCE_PASSWORD=root
ENV SPRING_JPA_SHOW_SQL=true
ENV SPRING_DATASOURCE_DRIVER_CLASS_NAME=com.mysql.cj.jdbc.Driver

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "/app/roomie.jar"]

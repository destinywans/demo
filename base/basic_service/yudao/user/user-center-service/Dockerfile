FROM 10.101.2.123/library/brand-maven-demo:v8

WORKDIR /opt/user-center-service

COPY ./target/user-center-service-1.0-SNAPSHOT.jar .

EXPOSE 9497

ENTRYPOINT ["java", "-jar", "user-center-service-1.0-SNAPSHOT.jar"]

CMD [""]
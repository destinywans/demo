from 10.101.2.123/cache/brand-java8-base:v1.0

workdir /opt/basic-platform-service

copy ./basic-platform-service/target/basic-platform-service-1.0-SNAPSHOT.jar .

expose 8080

entrypoint ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "basic-platform-service-1.0-SNAPSHOT.jar"]

cmd [""]
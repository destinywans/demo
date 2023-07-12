from 10.101.2.123/library/brand-maven-demo:v8

workdir /opt/basic-platform-service

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

copy ./basic-platform-service/basic-platform-service-1.0-SNAPSHOT.jar .

expose 8080

entrypoint ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "basic-platform-service-1.0-SNAPSHOT.jar"]

cmd [""]
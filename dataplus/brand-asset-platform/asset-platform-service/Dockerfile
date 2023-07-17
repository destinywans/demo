from 10.101.2.123/library/brand-maven-demo:v8

workdir /opt/asset-platform-service

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

copy ./basic-platform-service/target/asset-platform-service-1.0-SNAPSHOT.jar .

expose 9530

entrypoint ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "asset-platform-service-1.0-SNAPSHOT.jar"]

cmd [""]
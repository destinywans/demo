FROM 10.101.2.123/library/brand-maven-demo:v8

WORKDIR /opt/user-center-service

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

COPY ./target/user-center-service-1.0-SNAPSHOT.jar .

EXPOSE 9497

ENTRYPOINT ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "-Dspring.profiles.active=dev", "user-center-service-1.0-SNAPSHOT.jar"]

CMD [""]
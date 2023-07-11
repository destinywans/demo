FROM 10.101.2.123/library/brand-maven-demo:v8

WORKDIR /opt/inner-gateway

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

COPY ./target/inner-gateway-1.0-SNAPSHOT.jar .

EXPOSE 9997

ENTRYPOINT ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "-Dspring.profiles.active=dev", "-Djava.security.egd=file:/dev/./urandom", "inner-gateway-1.0-SNAPSHOT.jar"]

CMD [""]
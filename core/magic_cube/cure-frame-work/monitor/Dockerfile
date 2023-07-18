# FROM 10.101.2.123/library/brand-maven-demo:v8

FROM 10.101.2.123/cache/gongshu-maven-base:v2.0

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

WORKDIR /opt/monitor

EXPOSE 8091

COPY ./target/brand-boot-module-monitor-2.4.0.jar .

ENTRYPOINT ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "-Dspring.profiles.active=dev", "-Duser.timezone=GMT+08", "-Djava.security.egd=file:/dev/./urandom", "brand-boot-module-monitor-2.4.0.jar"]

CMD [""]
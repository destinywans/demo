FROM 10.101.2.123/library/brand-maven-demo:v8

# FROM 10.101.2.123/cache/gongshu-maven-base:v2.0

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

WORKDIR /opt/resource-management

EXPOSE 9500

COPY resource-management-service/target/resource-management-service-1.0-SNAPSHOT.jar .

RUN ls && pwd

ENTRYPOINT ["java", "-jar", "-Duser.timezone=Asia/Shanghai", "-Dspring.profiles.active=dev", "-Duser.timezone=GMT+08", "-Djava.security.egd=file:/dev/./urandom", "resource-management-service-1.0.SNAPSHOT.jar"]

CMD [""]
FROM maven:3.6.3-openjdk-11

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

WORKDIR /opt/keycloak

EXPOSE 8080

COPY settings.xml /root/.m2/

ENTRYPOINT ["java", "-jar", "-Dfile.encoding=utf-8", "-Duser.timezone=GMT+08", "demo-product-1.0-SNAPSHOT.jar"]

CMD [""]
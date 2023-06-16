FROM 10.101.2.123/cache/openjdk:8-jre

MAINTAINER wans

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

WORKDIR /opt/ws

EXPOSE 9060

COPY ./target/demo-product-1.0-SNAPSHOT.jar .

ENTRYPOINT ["java", "-jar", "-Dfile.encoding=utf-8", "-Duser.timezone=GMT+08", "demo-product-1.0-SNAPSHOT.jar"]

CMD [""]
ARG MAVEN_EXT_PARAM=''

FROM 10.101.2.123/library/brand-maven-demo:v8 as builder

WORKDIR /app

COPY /app/src /app

COPY /app/pom.xml /app

RUN mvn clean package $MAVEN_EXT_PARAM | ts '[%Y-%m-%d %H:%M:%S]' | tee /app/maven/demo-build.log

FROM openjdk:8-jre

MAINTAINER wans

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

WORKDIR /opt/ws

EXPOSE 9060

COPY --from=builder /app/target/demo-product-1.0-SNAPSHOT.jar .

ENTRYPOINT ["java", "-jar", "-Dfile.encoding=utf-8", "-Duser.timezone=GMT+08", "demo-product-1.0-SNAPSHOT.jar"]

CMD [""]
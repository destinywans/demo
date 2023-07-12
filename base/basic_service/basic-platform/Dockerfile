from 10.101.2.123/library/brand-maven-demo:v8

workdir /opt/basic-platform

copy ./target/basic-platform-1.0-SNAPSHOT.jar .

expose 8080

entrypoint ["java", "-jar", "basic-platform-1.0-SNAPSHOT.jar"]
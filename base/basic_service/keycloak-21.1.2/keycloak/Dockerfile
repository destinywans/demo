FROM maven:3.6.3-openjdk-11-slim

WORKDIR /opt/keycloak

COPY ./quarkus/dist/target/keycloak-21.1.2.tar.gz .

RUN tar -xfz keycloak-21.1.2.tar.gz

ENTRYPOINT ["./keycloak-21.1.2/bin/kc.sh", "start", "--hostname-url=http://10.101.3.200:8080/", "--http-enabled", "true", "--db", "mysql", "--db-url", "jdbc:mysql://mysql-headless.mysql:3306/keycloak_prd", "--db-username", "root", "--db-password", "1234qwer"]

CMD [""]
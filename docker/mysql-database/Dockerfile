FROM mysql:latest

ADD  docker-entrypoint-initdb.d/ /docker-entrypoint-initdb.d/

ENV MYSQL_DATABASE=tomcat
ENV MYSQL_USER=rest
ENV MYSQL_PASSWORD=pw
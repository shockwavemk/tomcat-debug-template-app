FROM tomcat:7-jre8
MAINTAINER Martin Kramer <info@martin-kramer.com>

ADD tomcat/tomcat-users.xml $CATALINA_HOME/conf/

ADD tomcat/run.sh $CATALINA_HOME/bin/run.sh
RUN chmod +x $CATALINA_HOME/bin/run.sh
ADD tomcat/mysql-connector-java-5.1.36-bin.jar $CATALINA_HOME/lib/

RUN rm -rf /usr/local/tomcat/webapps/ROOT

ENV JPDA_ADDRESS="8000"
ENV JPDA_TRANSPORT="dt_socket"

EXPOSE 8080
CMD ["run.sh"]

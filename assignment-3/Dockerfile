FROM ubuntu:18.04
MAINTAINER vinod
RUN apt-get update -y && apt-get install tomcat9 -y
RUN service tomcat start
COPY game-of-life.war /usr/local/tomcat/webapps
EXPOSE 8080
ENTRYPOINT /usr/local/tomcat/bin/catalina.sh run

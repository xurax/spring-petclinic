# INSTRUCTIONS
FROM centos:latest
MAINTAINER mmakhli
RUN yum -y install java-1.8.0-openjdk-devel.x86_64 
RUN yum -y install tomcat
ENV NAME whatever
RUN mkdir /logs
CMD tomcat start && tail -f /logs/catalina.out
ADD *.war /usr/share/tomcat/webapps

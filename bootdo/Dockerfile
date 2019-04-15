FROM 10.45.80.1/public/centos7_java8_tomcat8_base:8.0.35
MAINTAINER gengbin
COPY bootdo-2.0.0.jar /usr/tomcat/tomcat8.0/webserver/webapps/bootdo-2.0.0.jar
EXPOSE 8080
RUN yum -y install curl  \
        && yum clean all    \
        && chmod +x /usr/tomcat/tomcat8.0/webserver/bin/*.sh
CMD ["start"]
#ENTRYPOINT ["java","-jar","/bootdo-2.0.0.jar"]
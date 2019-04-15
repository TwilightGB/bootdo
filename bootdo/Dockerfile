FROM 10.45.80.1/public/centos7_java8_tomcat8_base:8.0.35
MAINTAINER gengbin
COPY bootdo/target/bootdo-2.0.0.jar /usr/tomcat/tomcat8.0/webserver/webapps
EXPOSE 8080
RUN chmod +x /usr/tomcat/tomcat8.0/webserver/bin/*.sh
CMD ["start"]
#ENTRYPOINT ["java","-jar","/bootdo-2.0.0.jar"]
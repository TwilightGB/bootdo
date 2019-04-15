#FROM 10.45.80.1/public/centos7_java8_tomcat8_base:8.0.35
FROM 10.45.80.1/public/centos7-java-base:openjdk1.8.0.151
MAINTAINER gengbin
#COPY ./bootdo-2.0.0.jar /usr/tomcat/tomcat8.0/webserver/webapps
COPY ./bootdo-2.0.0.jar /root/lib/
EXPOSE 8080
RUN mkdir -p /root/logs \
    && chmod +x /root/docker-app.def

ENV APP_NAME=bootdo

ENTRYPOINT ["/usr/local/bin/tini", "-g", "--", "docker-entrypoint.sh"]
CMD ["start"]
#ENTRYPOINT ["java","-jar","/bootdo-2.0.0.jar"]
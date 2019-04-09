FROM 10.45.80.1/public/centos7-java-base:openjdk1.8.0.151
MAINTAINER gengbin
ADD ./target/lib/bootdo-2.0.0.jar bootdo.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","/bootdo.jar"]
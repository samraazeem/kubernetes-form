FROM tomcat:8.5.11
MAINTAINER Samra Azeem

#RUN apt-get update && apt-get install -y \nano\&& mkdir -p /usr/local/tomcat/conf
COPY tomcat-users.xml /usr/local/tomcat/conf/
COPY context.xml /usr/local/tomcat/webapps/manager/META-INF/
ADD target/springmvcform.war /usr/local/tomcat/webapps/
EXPOSE 8080
CMD ["catalina.sh", "run"]

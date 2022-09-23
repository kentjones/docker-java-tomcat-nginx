FROM tomcat:8.5.5-jre8

LABEL maintainer="nite.coder@use.startmail.com"

COPY conf/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
COPY conf/context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml

# could create the war file from another dockerfile
COPY webapps/sample.war /usr/local/tomcat/webapps/

EXPOSE 5000

WORKDIR /usr/local/tomcat
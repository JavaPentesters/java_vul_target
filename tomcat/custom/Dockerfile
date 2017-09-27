FROM ubuntu:14.04
MAINTAINER pez1420 pez1420@gmail.com

#http://archive.apache.org/dist/tomcat/
ADD jdk-7u45-linux-x64.tar.gz /usr/local/
ADD apache-tomcat-7.0.73.tar.gz /usr/local/

ENV JAVA_HOME /usr/local/jdk1.7.0_45
ENV CLASSPATH $JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
ENV CATALINA_HOME /usr/local/apache-tomcat-7.0.73
ENV CATALINA_BASE /usr/local/apache-tomcat-7.0.73
ENV PATH $PATH:$JAVA_HOME/bin:$CATALINA_HOME/lib:$CATALINA_HOME/bin

CMD ["/usr/local/apache-tomcat-7.0.73/bin/catalina.sh", "run"]
EXPOSE 8080
FROM codenvy/jdk7
MAINTAINER pez1420 pez1420@gmail.com

ADD spring-data-rest-cve-2017-8046.jar /usr/local

WORKDIR /usr/local
CMD ["nohup","java", "-jar","spring-data-rest-cve-2017-8046.jar", "&"]
EXPOSE 8080
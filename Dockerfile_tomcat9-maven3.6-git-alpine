FROM tomcat:9-jre8-alpine

#install maven to /tools/maven
RUN wget http://mirror.navercorp.com/apache/maven/maven-3/3.6.0/binaries/apache-maven-3.6.0-bin.tar.gz
RUN tar -xvzf apache-maven-3.6.0-bin.tar.gz
RUN mkdir /tools
RUN mv ./apache-maven-3.6.0 /tools
RUN ln -s /tools/apache-maven-3.6.0 /tools/maven

#install tools for dev
RUN apk add openjdk8
RUN apk add git
RUN apk add nmap
RUN apk add htop
RUN apk add vim

FROM ubuntu:14.04
MAINTAINER onishishigure@gmail.com

RUN apt-get update

RUN \ 
  apt-get install -y wget openjdk-7-jre-headless && \
  wget https://download.elastic.co/elasticsearch/elasticsearch/elasticsearch-1.5.2.tar.gz && \
  tar zxf elasticsearch-1.5.2.tar.gz && \
  rm -rf elasticsearch-1.5.2.tar.gz

EXPOSE 9200

ENTRYPOINT ["/elasticsearch-1.5.2/bin/elasticsearch"]

FROM ubuntu:14.04
MAINTAINER onishishigure@gmail.com

RUN apt-get update

RUN \
  apt-get install -y wget && \ 
  wget https://download.elastic.co/kibana/kibana/kibana-4.0.2-linux-x64.tar.gz && \
  tar zxf kibana-4.0.2-linux-x64.tar.gz && \
  rm -rf /kibana-4.0.2-linux-x64.tar.gz

ENTRYPOINT ["/kibana-4.0.2-linux-x64/bin/kibana"]

FROM ubuntu:14.04
MAINTAINER onishishigure@gmail.com

RUN apt-get update

RUN \
  apt-get install -y curl && \
  curl -L https://td-toolbelt.herokuapp.com/sh/install-ubuntu-trusty-td-agent2.sh | sh

RUN \
  /opt/td-agent/usr/sbin/td-agent-gem install fluent-plugin-elasticsearch

ENTRYPOINT ["/usr/sbin/td-agent"]

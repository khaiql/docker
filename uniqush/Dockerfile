
FROM ubuntu:14.04

RUN apt-get update

RUN apt-get -q -y install redis-server
RUN apt-get -q -y install wget
RUN cd /tmp && wget http://uniqush.org/downloads/uniqush-push_2.1.0_amd64.deb
RUN cd /tmp && dpkg -i uniqush-push_2.1.0_amd64.deb
RUN /etc/init.d/redis-server start

CMD uniqush-push


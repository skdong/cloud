FROM cloud/centos7/base:latest
MAINTAINER "kaidong" <shikaidong@live.com>
ENV container docker
#install develop lib
RUN yum -y install bind-utils bind
RUN systemctl enable named
VOLUME [ "/sys/fs/cgroup" ]
CMD ["/usr/sbin/init"]

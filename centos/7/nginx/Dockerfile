FROM cloud/centos7/develop:latest
MAINTAINER "kaidong" <shikaidong@live.com>
ENV container docker
#cp openresty repo to image
COPY OpenRestry.repo /etc/yum.repos.d
RUN yum -y install openresty
VOLUME [ "/sys/fs/cgroup" ]
CMD ["/usr/sbin/init"]

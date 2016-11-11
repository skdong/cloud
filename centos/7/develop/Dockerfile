FROM cloud/centos7/base:latest
MAINTAINER "kaidong" <shikaidong@live.com>
ENV container docker
#install develop lib
RUN yum -y install python-openstackclient openstack-selinux svn python-pip; \
yum -y install python-devel mariadb-devel gcc iproute net-tools vim tcpdump;\
#update pip
pip install -U pip;

VOLUME [ "/sys/fs/cgroup" ]
CMD ["/usr/sbin/init"]

FROM cloud/centos7/develop:latest
MAINTAINER "kaidong" <shikaidong@live.com>
ENV container docker
#copy project to images
COPY cloud_portal /root/cloud_portal
#install python depandence lib
RUN yum -y install git ;\
for project in leopard marmot millet hedwig sloth inkfish lotus sinnet_www ;\
do \
pip install -r /root/cloud_portal/$project/requirements.txt ;\
done

VOLUME [ "/sys/fs/cgroup" ]
CMD ["/usr/sbin/init"]

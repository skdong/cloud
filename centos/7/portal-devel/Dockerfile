FROM cloud/centos7/portal-base
MAINTAINER "kaidong" <shikaidong@live.com>
ENV container docker
install python depandence lib
RUN for project in leopard marmot millet hedwig sloth inkfish lotus sinnet_www ;\
do \
pip install -r /root/cloud_portal/$project/requirements.txt ;\
done
VOLUME [ "/sys/fs/cgroup" ]
CMD ["/usr/sbin/init"]

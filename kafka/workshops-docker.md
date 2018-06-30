
# Docker

+++
### Docker
przed
~~~bash
cd ../HADOOP/docker/kafka/1_1_0/cluster
docker-compose up
~~~
na sam koniec
~~~bash
docker-compose down
~~~


+++
### Docker
bash kontenera
~~~bash
docker exec -it cluster_kafka1 bash
cd /opt/kafka_2.12-1.1.0/
~~~



+++
### Hosty
~~~bash
./check-hosts.sh 
172.22.0.0/16 dev eth0  proto kernel  scope link  src 172.22.0.2 
172.22.0.0/16 dev eth0 scope link  src 172.22.0.3 
172.22.0.0/16 dev eth0 scope link  src 172.22.0.4 
172.22.0.0/16 dev eth0 scope link  src 172.22.0.5 
~~~

~~~bash
cat /etc/hosts | grep cluster
172.22.0.2 cluster_zookeeper
172.22.0.3 cluster_kafka1
172.22.0.4 cluster_kafka2
172.22.0.5 cluster_kafka3
~~~
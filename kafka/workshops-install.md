
# Instalacja

+++
### Paczka Apache
~~~bash
mkdir kafka
cd kafka
wget http://ftp.man.poznan.pl/apache/kafka/1.1.0/kafka_2.11-1.1.0.tgz
tar -xzf kafka_2.11-1.1.0.tgz
~~~

+++
### Uruchomienie ZooKeepera
~~~bash
cd kafka_2.11-1.1.0/
bin/zookeeper-server-start.sh config/zookeeper.properties
~~~

+++
### Uruchomienie brokera
~~~bash
bin/kafka-server-start.sh config/server.properties
~~~



+++
### Konfiguracja
https://kafka.apache.org/documentation/#brokerconfigs
* cleanup.policy=compact
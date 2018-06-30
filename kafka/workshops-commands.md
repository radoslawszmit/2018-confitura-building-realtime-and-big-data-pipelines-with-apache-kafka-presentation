
# Podstawowe operacje w konsoli


+++
### Docker
~~~bash
docker-compose up
docker exec -it cluster_kafka1 bash
cd /opt/kafka_2.12-1.1.0/
~~~



+++
### Zmienne systemowe
~~~bash
export KAFKA_ZOOKEEPER=localhost:2181
export KAFKA_BROKER=localhost:9092
export TOPIC=test-topic
~~~
lub
~~~bash
export KAFKA_ZOOKEEPER=cluster_zookeeper:2181
export KAFKA_BROKER=cluster_kafka1:9092,cluster_kafka2:9092,cluster_kafka3:9092
export TOPIC=test-topic
~~~


+++
### Stworzenie topicu
~~~bash
bin/kafka-topics.sh --create --zookeeper $KAFKA_ZOOKEEPER \
    --replication-factor 1 --partitions 1 --topic $TOPIC
~~~


+++
### Informacje o topicu
~~~bash
bin/kafka-topics.sh --describe --zookeeper $KAFKA_ZOOKEEPER
bin/kafka-topics.sh --describe --zookeeper $KAFKA_ZOOKEEPER \
    --topic $TOPIC
bin/kafka-topics.sh --zookeeper $KAFKA_ZOOKEEPER --describe \
    --under-replicated-partitions
~~~


+++
### Edycja topicu
~~~bash
bin/kafka-topics.sh --alter --zookeeper $KAFKA_ZOOKEEPER \
    --topic $TOPIC --partitions 3
~~~


+++
### Lista topiców
~~~bash
bin/kafka-topics.sh --list --zookeeper $KAFKA_ZOOKEEPER
~~~
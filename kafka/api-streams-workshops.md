
# Streams API
# Warsztat


+++
### Wynik z Kafka Streams
~~~bash
bin/kafka-console-consumer.sh --bootstrap-server $KAFKA_BROKER --topic $TOPIC --from-beginning

bin/kafka-console-consumer.sh --bootstrap-server $KAFKA_BROKER \
    --topic test-topic-out \
    --from-beginning \
    --formatter kafka.tools.DefaultMessageFormatter \
    --property print.key=true \
    --property print.value=true \
    --property key.deserializer=org.apache.kafka.common.serialization.StringDeserializer \
    --property value.deserializer=org.apache.kafka.common.serialization.StringDeserializer
~~~
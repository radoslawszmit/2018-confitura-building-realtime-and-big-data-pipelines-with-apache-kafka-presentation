
# Producer API
# Consumer API

+++
### Producer API
~~~java
Properties producerConfig = new Properties();
producerConfig.put(ProducerConfig.BOOTSTRAP_SERVERS_CONFIG, KAFKA_SERVER);
producerConfig.put(ProducerConfig.ACKS_CONFIG, "all");
producerConfig.put(ProducerConfig.RETRIES_CONFIG, 0);
producerConfig.put(ProducerConfig.VALUE_SERIALIZER_CLASS_CONFIG, StringSerializer.class.getCanonicalName());
producerConfig.put(ProducerConfig.KEY_SERIALIZER_CLASS_CONFIG, StringSerializer.class.getCanonicalName());

Producer<String, String> producer = new KafkaProducer<>(producerConfig);

ProducerRecord<String, String> data = new ProducerRecord<>(TOPIC, MESSAGE_ID, "Message text...");
producer.send(data);
~~~
@[1-6](Konfiguracja)
@[8](Kafka producent)
@[10](Rekord wiadomośći (klucz - wartość))
@[11](Wysłanie wiadomości)



+++
### Consumer API
~~~java
Properties consumerConfig = new Properties();
consumerConfig.put(ConsumerConfig.BOOTSTRAP_SERVERS_CONFIG, KAFKA_SERVER);
consumerConfig.put(ConsumerConfig.GROUP_ID_CONFIG, "group-name");
consumerConfig.put(ConsumerConfig.AUTO_OFFSET_RESET_CONFIG, "earliest");
consumerConfig.put(ConsumerConfig.VALUE_DESERIALIZER_CLASS_CONFIG, StringDeserializer.class.getCanonicalName());
consumerConfig.put(ConsumerConfig.KEY_DESERIALIZER_CLASS_CONFIG, StringDeserializer.class.getCanonicalName());

KafkaConsumer<String, String> consumer = new KafkaConsumer<>(consumerConfig);
consumer.subscribe(Collections.singletonList(TOPIC));

ConsumerRecords<String, String> records = consumer.poll(TIMEOUT);

if (records.count() > 0) {
    LOGGER.info("Poll records: " + records.count());

    for (ConsumerRecord<String, String> record : records) {
        System.out.printf("Received Message topic = %s, partition = %s, offset = %d, key = %s, value = %s\n",
        record.topic(), record.partition(), record.offset(), record.key(), record.value());
    }
}

consumer.commitAsync();
~~~
@[1-6](Konfiguracja)
@[8](Kafka konsument)
@[9](Subskrybcja do kolejki)
@[11](Pobranie wiadomości z topicu)
@[13-20](Pobranie wiadomości z topicu)
@[22](Offsets commit)
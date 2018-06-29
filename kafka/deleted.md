
### Deleted slides
not used in presentation


+++
### Confluent Platform
![](assets/img/distribution/confluentPlatform3.1.png)


+++
### Data copying

@div[left-50 fragment]
![](assets/img/architecture/traditional-data-copying.gif)
@divend

@div[right-50 fragment]
![](assets/img/architecture/zero-copy-data-copying.gif)
@divend



+++
### Context switching

@div[left-50 fragment]
![](assets/img/architecture/traditional-context-switching.gif)
@divend

@div[right-50 fragment]
![](assets/img/architecture/zero-copy-context-switching.gif)
@divend



+++
### Optymalizacja
* Java 1.8 z G1 collector
* Zostawić RAM dla “page chache’a”
* Zwiększyć liczbę deskryptorów
* High Performance Data Transfers (TCP)
* Używać dysków na wyłączność, używać wielu dysków, lepiej szybsze dyski
* Zookeeper powinien być na innych maszynach, większa wydajność przy wyłącznym korzystaniu
* RAID nie jest zalecany
* Zalecany jest EXT4 lub XFS
* Nie używać dysków współdzielonych/sieciowych (kafka doznaje awarii)


+++
### Ekosystem
* Integracja z narzędziami **Big Data**: Hadoop, Flume, JDBC, Elasticsearch, Presto, Hive, Camel etc.
* Integracja z narzędziami do **przetwarzania strumieniowego**: Spark, Storm, Samza, Flink, NiFi, Apex, Spring Cloud Stream etc.
* Dostępna w większości **dystrybucjach Big Data** (Cloudera, Hortonworks)
* Integracja z AWS i innymi **chmurami publicznymi**
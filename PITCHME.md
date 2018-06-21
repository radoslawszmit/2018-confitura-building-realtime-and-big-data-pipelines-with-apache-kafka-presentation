
# Building Realtime & Big Data Pipelines with Apache Kafka



---
# Radosław Szmit
@fa[twitter] @RadoslawSzmit <br/>
@fa[globe] http://bigdatapassion.pl/ </br>
@fa[envelope] radoslaw.szmit@gmail.com <br/>


---
### Czy jest Apache Kafka?
Apache Kafka® is a distributed streaming platform


---
### Czy jest Apache Kafka?
* Kolejka danych (Publish + Subscribe)
* Rozproszona “baza danych” (distributed commit log)
* Przetwarzanie strumieniowe danych


---
### Zastosowania
* Narzędzie do efektywnego strumieniowego przesyłania danych pomiędzy systemami i aplikacjami 
* Narzędzie do przetwarzania strumieni danych
* Narzędzie do reagowania na zdarzenia



---
### Zastosowania
![](img/chart-kafka-infrastructure.png)



---
### Cechy
* Narzędzie (niemal) czasu rzeczywistego
* Narzędzie Big Data (terabajty danych, miliony zdarzeń na sekundę)



---
### Popularność w świecie Big Data
![](img/five-years-of-hadoop-weekly.png)
<span class="footer">https://medium.com/@joecrobak/five-years-of-hadoop-weekly-7aa8994f140b</span>



---
### Kafka API

@div[left-50]
![](img/kafka-apis.png)
@divend

@div[right-50]
@ul[white]
- Producer API
- Consumer API
- Streams API
- Connect API
- AdminClient API
- Legacy API (old)
@ulend
@divend



---
### Klienci Kafka
* Zespół Apache Kafka utrzymuje i rozwija bibliotekę kliencką dla języka **Java**
* Dostępne są klienci "community" dla innych języków: C/C++, Python, Go (AKA golang), Erlang, .NET, Clojure, Ruby, Node.js, Proxy (HTTP REST, etc), Perl, stdin/stdout, PHP, Rust, Alternative Java, Storm, Scala DSL, Clojure, Swift etc.



---
### Ekosystem
* Integruje się z wieloma narzędziami: Hadoop, Flume, JDBC, Elasticsearch, Presto, Hive, Camel etc.
* Integracja z narzędziemi do przetwarzania strumieniowego: Spark, Storm, Samza, Flink, Apex, Spring Cloud Stream etc.
* Dystrybucje Big Data (Cloudera, Hortonworks)
* Integracja z AWS



---
### Kafka Logs
![](img/log_consumer.png)



---
### Partycje
![](img/log_anatomy.png)



---
### Grupy konsumentów
![](img/consumer-groups.png)



---
### Zero-copy
"Zero-copy" describes computer operations in which the CPU does not perform the task of copying data from one memory area to another. This is frequently used to save CPU cycles and memory bandwidth when transmitting a file over a network. Wikipedia



---
### Data copying

@div[left-50 fragment]
![](img/traditional-data-copying.gif)
@divend

@div[right-50 fragment]
![](img/zero-copy-data-copying.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>



---
### Context switching

@div[left-50 fragment]
![](img/traditional-context-switching.gif)
@divend

@div[right-50 fragment]
![](img/zero-copy-context-switching.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>




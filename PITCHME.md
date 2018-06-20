
### Building Realtime & Big Data Pipelines with Apache Kafka


---

Apache Kafka® is a distributed streaming platform


---

* Kolejka danych (Publish + Subscribe)
* Rozproszona “baza danych” (distributed commit log)
* Przetwarzanie strumieniowe danych


---

* Narzędzie do efektywnego strumieniowego przesyłania danych pomiędzy systemami i aplikacjami 
* Narzędzie do przetwarzania strumieni danych


---

* Narzędzie (niemal) czasu rzeczywistego
* Big Data (terabajty danych, miliony zdarzeń na sekundę)




---?

### Kafka API

@div[left-50]
<br>
![MONKEY](img/kafka-apis.png)
@divend
<br/><br/>
@div[right-50]
@ul[white]
- Producer API
- Consumer API
- Streams API
- Connector API
@ulend
@divend




---


* Można używać wielu języków programowania (główny Scala)
* Integruje się z wieloma narzędziami (np. Storm i Spark)
* Używa mechanizmu “Zero Copy”
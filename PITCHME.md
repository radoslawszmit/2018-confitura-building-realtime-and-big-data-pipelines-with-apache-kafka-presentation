
### Building Realtime & Big Data Pipelines
### with Apache Kafka


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
### Cechy
* Narzędzie (niemal) czasu rzeczywistego
* Narzędzie Big Data (terabajty danych, miliony zdarzeń na sekundę)



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
* Integruje się z wieloma narzędziami (np. Storm i Spark)



---?image=img/log_consumer.png&size=auto 50%&position=center

### Kafka Logs



---?image=img/log_anatomy.png&size=auto 50%&position=center
### Partycje


---
### Partycje
![](img/log_anatomy.png)



---?image=img/consumer-groups.png&size=auto 50%&position=center
### Grupy konsumentów



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
![](img/traditional-data-copying.gif)
@divend

@div[right-50 fragment]
![](img/zero-copy-data-copying.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>




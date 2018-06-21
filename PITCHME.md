
### Building Realtime & Big Data Pipelines
### with Apache Kafka


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



---?image=img/log_anatomy.png&size=auto 50%&position=center



---?image=img/log_consumer.png&size=auto 50%&position=center



---

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



---
* Można używać wielu języków programowania (główny Scala)
* Integruje się z wieloma narzędziami (np. Storm i Spark)
* Używa mechanizmu “Zero Copy”
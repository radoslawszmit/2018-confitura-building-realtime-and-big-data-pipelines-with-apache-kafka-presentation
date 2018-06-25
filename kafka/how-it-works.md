
# Zasada działania


---
### Kafka Logs
![](img/how-it-works/log.png)



---
### Kafka Logs
* Prosta abstrakcja składowania danych
* Logi to wiadomości klucz-wartość
* Sekwencja danych (zachowuje kolejność)
* Brak edycji (tylko append)
* Logi danych a nie aplikacji (!=log4j)



---
### Producenci i konsumenci logów
![](img/how-it-works/kafka-architecture.png)



---
### Producenci i konsumenci logów
![](img/how-it-works/log_subscription.png)



---
### Partycje
![](img/how-it-works/partitioned_log.png)



---
### Partycje
![](img/how-it-works/log_anatomy.png)



---
<!-- .slide: class="imagecentersize50" -->
### Consumer offset
![](img/how-it-works/log_consumer.png)



---
### Grupy konsumentów
![](img/how-it-works/consumer-group.png)



---
### Grupy konsumentów
![](img/how-it-works/consumer-groups.png)



---
### Kompaktowanie logów
![](img/how-it-works/log_compaction_0.png)
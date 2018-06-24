
# Zasada działania


+++
### Kafka Logs
![](img/how-it-works/log.png)



+++
### Kafka Logs
* Prosta abstrakcja składowania danych
* Sekwencja danych (zachowuje kolejność)
* Brak edycji (tylko append)
* Logi danych a nie aplikacji (!=log4j)
* Logi to wiadomości klucz-wartość


+++
### Producenci i konsumenci logów
![](img/how-it-works/log_subscription.png)


+++
### Partycje
![](img/how-it-works/partitioned_log.png)


+++
### Partycje
![](img/how-it-works/log_anatomy.png)



+++
### Consumer offset
![](img/how-it-works/log_consumer.png)



+++
### Grupy konsumentów
![](img/how-it-works/consumer-groups.png)



+++
### Kompaktowanie logów
![](img/how-it-works/log_compaction_0.png)

# Zasada działania


+++
### Kafka Logs

@div[left-50]
![](img/how-it-works/log_consumer.png)
@divend

@div[right-50]
@ul
* Prosta abstrakcja składowania danych
* Sekwencja danych (zachowuje kolejność)
* @size[0.5em](Brak edycji (tylko append))
* Brak edycji (tylko append)
* Logi danych a nie aplikacji (!=log4j)
@ulend
@divend



+++
### Kafka Logs
![](img/how-it-works/log_consumer.png)



+++
### Kafka Logs
* Prosta abstrakcja składowania danych
* Sekwencja danych (zachowuje kolejność)
* Brak edycji (tylko append)
* Logi danych a nie aplikacji (!=log4j)



+++
### Partycje
![](img/how-it-works/log_anatomy.png)



+++
### Grupy konsumentów
![](img/how-it-works/consumer-groups.png)
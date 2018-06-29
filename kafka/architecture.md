
# Architektura


+++
### Architektura
![](assets/img/architecture/Kafka-Broker-Diagram.png)



+++
### Brokerzy
![](assets/img/architecture/broker-on-disk.png)



+++
### Wiadomości
![](assets/img/architecture/messages.jpg)



+++
### Segmenty
![](assets/img/architecture/segments.png)


+++
### Zero-copy
"Zero-copy" describes computer operations in which the CPU does not perform the task of copying data from one memory area to another. This is frequently used to save CPU cycles and memory bandwidth when transmitting a file over a network. Wikipedia



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

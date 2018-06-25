
# Architektura


---
### Architektura
![](img/architecture/Kafka-Broker-Diagram.png)



---
### Brokerzy
![](img/architecture/broker-on-disk.png)



---
### Wiadomości
![](img/architecture/messages.jpg)



---
### Segmenty
![](img/architecture/segments.png)


---
### Zero-copy
"Zero-copy" describes computer operations in which the CPU does not perform the task of copying data from one memory area to another. This is frequently used to save CPU cycles and memory bandwidth when transmitting a file over a network. Wikipedia



---
### Data copying

@div[left-50 fragment]
![](img/architecture/traditional-data-copying.gif)
@divend

@div[right-50 fragment]
![](img/architecture/zero-copy-data-copying.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>



---
### Context switching

@div[left-50 fragment]
![](img/architecture/traditional-context-switching.gif)
@divend

@div[right-50 fragment]
![](img/architecture/zero-copy-context-switching.gif)
@divend

<span class="footer">https://www.ibm.com/developerworks/library/j-zerocopy/index.html</span>
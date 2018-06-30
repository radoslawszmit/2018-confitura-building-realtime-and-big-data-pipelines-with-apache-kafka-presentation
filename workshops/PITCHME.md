
## Introduction to streaming data and stream processing with Apache Kafka



---?include=kafka/sponsors.md
---?include=kafka/about.md



---
### Cel prezentacji
* Poznanie Apache Kafka
* Umiejętność wykorzystania w praktyce



---
## Nauczycielem wszystkiego jest praktyka
Gajusz Juliusz Cezar



---
### Organizacyjnie
@fa[clock-o] Warsztat 4h (14 - 18) <br />
@fa[question] Pytania i problemy na bieżąco <br />
@fa[coffee] Krótkie przerwy w trakcie @fa[smile-o] <br />



---
### Tematyka
<!-- .slide: class="font80" -->
1. Introduction
    1. History
    1. Use cases
    1. Terminology
    1. Architecture
    1. Comparison between Kafka and Message Queues
1. APIS
    1. Producer API
    1. Consumer API
    1. Streams API
    1. Message serialization
1. Operations
    1. Installation
    1. Configuration
    1. Replication
    1. Data compression


---
### Harmonogram
<!-- .slide: class="font80" -->
* Wstęp
* Środowisko pracy
* Podstawowe operacje w konsoli
* Producer / Consumer API
* Odporność na awarie (crash testy)
* Kafka Streams API
* Podsumowanie



---
### GitHub
https://github.com/sagespl/HADOOP
~~~bash
git clone https://github.com/sagespl/HADOOP.git
cd HADOOP
mvn clean install -DskipTests=true
~~~



---
<!-- .slide: class="font80" -->
### Środowisko Developerskie
* Własne środowisko
    * IntelliJ IDEA (Community lub Ultimate)
    * Java (JDK) 8
    * Scala 2.11
    * Maven 3.5+
    * Git
    * Docker CE 18+
    * Docker Compose 1.20+
* Gotowe środowisko
    * VirtualBox 5.2+
    * Windows/Linux/Mac 64 bit
    * virtualization enabled in PC BIOS


---?include=kafka/intro-mini.md
---?include=kafka/how-it-works.md
---?include=kafka/architecture.md
---?include=kafka/integration.md
---?include=kafka/api-publish-subscribe.md
---?include=kafka/api-publish-subscribe-code.md
---?include=kafka/api-streams.md

---?include=kafka/guarantees.md

---?include=kafka/summary.md
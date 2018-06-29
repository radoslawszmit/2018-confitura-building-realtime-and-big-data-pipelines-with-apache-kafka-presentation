
# Gwarancje dostarczenia


+++
#### There are only two hard things in Computer Science: 
#### cache invalidation and naming things.
-- Phil Karlton



+++
### Gwarancja dostarczenia
* At most once — Co najwyżej raz
* At least once — Przynajmniej raz
* Exactly once — Dokładnie raz



+++
### Gwarancja dostarczenia
* Kafka Streams wspiera exactly-once delivery 
* Pozostałe API domyślnie wspierają at-least-once delivery
* Exactly-once delivery wymaga współpracy z systemem docelowym, dodatkowa implementacja
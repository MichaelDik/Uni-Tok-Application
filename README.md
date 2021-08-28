# Distributed-Systems
---
## General Informations

Λόγω των περιοσμένων επιδόσεων των υπολογιστών μας συγκριτικά με τις απαιτήσεις της εφαρμογής (1 address keeper, 2 emulator και 3 broker) τεστάραμε τον κώδικά μας σε 1 address keeper, 3 broker, 1 emulator και σε 1 AppNodeImpl (από το 1ο project). Αναπόφευκτα έγιναν κάποιες τυπικές αλλαγές στο 1 μέρος. 

Για την εκτέλεση της εφαρμογής απαιτούνται τα εξής:
1) Run Address Keeper
2) Run BrokerImpl1 (set port 4221)
3) Run BrokerImpl2 (set port 4321)
4) Run BrokerImpl3 (set port 4421)
5) Run AppNodeImpl1 (1o project)
6) Run Emulator (2o project)
7) Για το redirection δες οδηγίες παρακάτω (στο Distributed-Systems-Part2) 
8) Η εφαρμογή είναι έτοιμη να τρέξει

---
## Distributed-Systems-Part1

Τυπικές αλλαγές ώστε να μπορεί να επικοινωνήσει χωρίς προβλήματα ένας AppNodeImpl (από το 1ο project) με έναν emulator.

---
## Distributed-Systems-Part2

Για την επιτυχή επικοινωνία μεταξύ broker και emulator θα πρέπει να γίνουν τα εξής:
1) Run Emulator 
2) Open Terminal and type:
    2.1) telnet localhost 5554
    2.2) auth "auth_token"
    2.3) redir add tcp:5529:4960

---

## Team

### Δημήτριος Αναστασόπουλος 3180010

### Μιχάλης Δικαιόπουλος 3180050

### Κωνσταντίνος Καρράς 3180076

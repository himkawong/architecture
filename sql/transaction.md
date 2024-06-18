## ACID

### Atomicity

* If several writes are grouped together into an atomic transaction, and the transaction cannot be completed due to a fault, then the transaction is aborted and the database must discard or undo any writes it has made so far in that transaction.

### Consistency

* A transaction should make no changes that violate the rules or constraint placed on the data. The application may rely on the database to archive consistency, but it's not up the database alone.

### Isolation

* Isolation in the sense of ACID means that concurrently executing transactions are isolated from each other: they cannot step on each other’s toes.

### Durability

* Once a transaction has committed succesfully, any data it has written will not be forgetten, even if there is hardware fault or the database crashes.


## Weak Isolation Level

* Read Committed
* Snapshot isolation (repeatable read)
* Serializable


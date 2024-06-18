## Distributed Lock

* Database: Distributed lock is generally not considered due to its poor performance in the database and the risk of locking the table.
  * Advantages: Simple to implement and easy to understand.
  * Disadvantages: High pressure on the database.
* Redis: Suitable for scenarios that require high concurrency and high performance. Its reliability could be compensated by other solutions.
  * Advantage: Easy to understand.
  * Disadvantages: Self-implemented and non-blocking.
* Redisson: Compared with Jedis, it is more used in distributed scenarios.
  * Advantage: Supports locking and blocking.
* ZooKeeper: Suitable for scenarios that require high reliability (high availability) but not for high concurrency.
  * Advantage: Supports blocking.
  * Disadvantages: high use threshold, complex.

  Reference:
  * https://redis.io/docs/latest/develop/use/patterns/distributed-locks/
  * https://medium.com/@wyr95626_29886/how-to-implement-a-distribue-lock-6d951a53e938


## Distributed Unique ID
  * UUID
  * Twitter's Snowflake
  
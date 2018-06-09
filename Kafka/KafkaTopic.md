## Kafka Topic ##

* Category or feed
* Each topic consist of Partitioned log (helps in horizontal Scaling)
* partition are ordered, immutable , sequence of messages appended
* Offset (sequential id ) assigned to each message in partition
* Kafka retains all the messages that are published regardless if they have been consumed or not,for a configurable period of time
* log retention : time messages will stay after published


## Kafka Broker ##

* Kafka cluster comprise of one or more servers -brokers
* Each kafka broker stores one or more partitions
*Single topic's partition can be spread over multiple broker
* Brokers are stateless
* Consumer has to keep track of offset


## Replication ##

* Each partition can be replicated across a number of servers
* Each partition has one "leader" and zero or more followers
* if leader fails, new leader elected
* leader keeps track of In-sync replicas(in track with leader)
* Committed messages are only consumed by kafka
* producers have option to wait for commit (latency vs durability)  

 

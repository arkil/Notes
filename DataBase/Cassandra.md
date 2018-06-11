## Cassandra ##

* Cassandra rows are organized into tables and indexed by a key 
* It uses append-only , log-based storage engine
* Data is distributed across master-less nodes ,with no single point failure 
* Nodes with in same data center share the same replication factor  or configuration
* Cassandra also provides network partition tolerance to heap tuning 
* Horizontal Scaling or scaling out
* multiple copies of data are stored on multiple nodes  
* Setting up nodes in corresponding  cloud regions can help improve application performance
* Cassandra will respond  to heap tuning for performance, and t allows to expose useful metrics and commands vis JMX
* If data is not persisted on disk , it is replayed from commit log


## Kafka Broker parameters ## 

* log.dirs (directory for logs)
* log.retention.hours (time for retention of message)
* log.roll.hours (force Kafka to roll a new log segment even if the log.segment.bytes size has not been reached.)
* zookeeper.connect (Specifies the zookeeper connection string)
* kafka.host (host port for kafka)

## Advance kafka broker parameters ##

* auto.create.topics.enable (kafka will create topic automatically when you send message to non existing topic)
* auto.leader.rebalance.enable (automatically rebalance when kafka is down)
* compression.type (type of compression for message)
* controlled.shutdown.enable (If enabled, the broker will move all leaders on it to some other brokers before shutting itself down)
* controlled.shutdown.max.retries (No of retries for shutdown)
* controlled.shutdown.retry.backoff.ms (back off time between entries)
* controller.message.queue.size (buffer size for controllerto broker)
* controller.socket.timeout.ms  (The socket timeout for commands from the partition management controller to the replicas.)

## other ##

max.message.bytes (size of message allowed on topic )


## producer configuration setting ##

* bootstrap.servers (host for connection to kafka cluster)
* client.id ( id can be passed )
* acks (no of acknowledgment to be received)
* retries (resend whose send fails)
* batch.size (collect messages . increase throughput )
* buffer.memory(limit total memory)
* linger.ms(producer to delay)
* compression.type (gzip/snappy)
* key.serializer / value.serializer (turn producer record to bytes)

## Consumer configuration settings

* enable.auto.commit (if true offset are automatically committed)
* auto.commit.interval.ms (commit frequency)
* bootstrap.servers (connection to kafka cluster) 
* client.id (tracking source requests)
* key.deserializer /value.deserializer (bytes to record)
* fetch.min.bytes (min amount of data to fetch a request)


 
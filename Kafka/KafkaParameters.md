## Kafka Broker parameters ## 

* log.dirs  : directory for logs
* log.retention.hours = time for retention of message
* log.roll.hours
* zookeeper.connect
* kafka.host

## Advance kafka broker parameters ##

* auto.create.topics.enable 
* auto.leader.rebalance.enable
* compression.type
* controlled.shutdown.enable
* controlled.shutdown.max.retries
* controlled.shutdown.retry.backoff.ms
* controller.message.queue.size
* controller.socket.timeout.ms  

## other ##

max.message.bytes = size of message allowed on topic


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


 
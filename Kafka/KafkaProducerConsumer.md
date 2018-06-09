## Kafka Producer ##

* Producer publish the message to a kafka  topic
* producers decides which message goes to which partition(round robin fashion)
* producers writes to single leader(load balancing)

## kafka Consumer ##

* consumer reads from topic
* Each message publish to a topic is deliver to one consumer instance in subscribing consumer group
* consumer instances per group can be on different machines
* consumer instances on same group have load balance 
* one consumer instance per partition
* consumer instance in different group subscribing to same topic can get copy of messages

## Zookeeper ## 

* kafka requires zookeeper 
* Zookeeper's responsibilities
	* clustering membership
	* electing a broker as controller
	* selecting leader , configuration of topic

## Kafka Key points ##

* messages are appended to partition in particular order
* consumer sees messages in order they are stored in log
* Committed messages are not lost as long as atleast one is in sync replica
* at least one (default) , at most one by disabling producer retries and committing offset prior to processing , exactly one requires destination storage

	

# Creating topic #

* First Run Zookeeper

run : zookeeper-server-start.sh
set properties in zookeper properties file

* start kafka server

run : kafka-server-start.sh 
pass server properties file

* create topic

if auto.create.topics.enable = true

topic is created automatically when broker receives message

or .

bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic topicname


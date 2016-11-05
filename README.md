# kafkatwitterproducer

This is a java program to write to kafka topic from twitter stream.

1.) Start Zookeeper
2.) Start Kafka - bin/kafka-server-start.sh config/server.properties
3.) Create topic - bin/kafka-topics.sh --create --topic twitterstreams --zookeeper localhost:2181 --partitions 1 --replication-factor 1
4.)Open consumer window terminal - bin/kafka-console-consumer.sh --topic itwitterstreams --zookeeper localhost:2181 

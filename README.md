# kafkatwitterproducer

This is a java program to write to kafka topic from twitter stream.


1.) Start Zookeeper

2.) Start Kafka - bin/kafka-server-start.sh config/server.properties

3.) Create topic - bin/kafka-topics.sh --create --topic twitterstreams --zookeeper localhost:2181 --partitions 1 --replication-factor 1

4.)Open consumer window terminal - bin/kafka-console-consumer.sh --topic itwitterstreams --zookeeper localhost:2181 

Compile using 

1) javac -cp "/home/navin/software/kafka/libs/*":"/home/navin/Downloads/twitter4j-4.0.4/lib/*":. KafkaTwitterProducer.java
2) java -cp "/home/navin/software/kafka/libs/*":"/home/navin/Downloads/twitter4j-4.0.4/lib/*":. KafkaTwitterProducer

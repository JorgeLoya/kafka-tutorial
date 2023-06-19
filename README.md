# kafka-tutorial
Simple project using SpringBoot and Kafka

Over time it will grow up

Commands on windows for Kafka:

Launch Zookeeper:  
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

Launch Kafka:  
.\bin\windows\kafka-topics.bat --create --topic {topic-name} --bootstrap-server {host}:9092

Details of Topic:  
.\bin\windows\kafka-topics.bat --describe --topic {topic-name} --bootstrap-server {host}:9092

List of created topics on the broker:  
.\bin\windows\kafka-topics.bat --list --bootstrap-server {host}:9092

Launch listener to see messages of specific topic:  
.\bin\windows\kafka-console-consumer.bat --topic {nombreTopic} --bootstrap-server {host}:9092

Launch console to send messages of specific topic:  
.\bin\windows\kafka-console-producer.bat --broker-list {host}:9092 --topic {topic-name}

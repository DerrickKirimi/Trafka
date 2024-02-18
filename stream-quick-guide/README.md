## **Apache Kafka Quick Reference - Work Done**  

Commands (This depends on the installation done)   

1). Start Zookeeper:  
```python
>>> kafka/bin/zookeeper-server-start.sh kafka/config/zookeeper.properties  
```
 

2). Start Kafka Server  

```python
>>> kafka/bin/kafka-server-start.sh kafka/config/server.properties   
```

3). Create Kafka Topic

```python 
>>> kafka-topics.sh --bootstrap-server IP:port --topic your_topic_name --create --partitions 3 --replication-factor 1
```

4). List Topics

```python
>>> kafka-topics.sh --list --bootstrap-server IP:port
```

5). Get a Topic Details ( --describe )

```python
>> kafka-topics.sh --describe --topic your_topic_name --bootstrap-server IP:port
```
>> To get deatails about all the --topic and topic name 

6). Create a simple Producer
```python
>>> kafka-console-producer.sh --broker-list IP:port --topic test_topic
```

7). Create a Simple Consumer 

```python
>>>  kafka-console-consumer.sh --bootstrap-server ip:port --topic test_topic --from-beginning
```

n). Stop Kafka Server   
```python
>>> kafka/bin/kafka-server-stop.sh kafka/config/server.properties  
```

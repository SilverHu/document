# kafka

## 查询集群描述

```
./kafka-topics.sh --zookeeper 127.0.0.1:2181 --describe
```

## 查询topic列表

```
./kafka-topics.sh --zookeeper 127.0.0.1:2181 --list
```

## 查询消费者列表

```
./kafka-consumer-groups.sh --bootstrap-server 10.226.20.105:9092 --list
```

## 查询消费详细

```
./kafka-consumer-groups.sh --bootstrap-server 10.226.20.105:9092 --group mobilecollect-consumer-group --describe
```

## 设置消费偏移量

```
# 设置为最初偏移量
./kafka-consumer-groups.sh --bootstrap-server 10.226.20.105:9092 --group mobilecollect-consumer-group --topic mobile_update_request --reset-offsets --to-earliest --execute

# 设置任意偏移量
./kafka-consumer-groups.sh --bootstrap-server 10.226.20.105:9092 --group mobilecollect-consumer-group --topic mobile_update_request --reset-offsets --to-offset 3 --execute
```
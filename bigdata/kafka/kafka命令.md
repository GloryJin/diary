# kafka命令

### Topic相关

1. 创建topic

   `./kafka-topics.sh  --create --zookeeper 10.47.222.239:2181/kafka --replication-factor 1 --partitions 1 --topic t_page_access`

2. 删除topic

   `./kafka-topics.sh --zookeeper 10.47.166.14:2181 --delete -topic t_logout`

3. 消费topic

   `./kafka-console-consumer.sh -zookeeper 10.47.166.14:2181 --from-beginning --topic t_logout`

4. 往topic插入数据

   `./kafka-console-producer.sh --broker-list 10.47.222.232:9092，10.47.222.239:9092 --topic t_logout `

5. 查看topic

   `./kafka-topics.sh  --list --zookeeper localhost:2181`





### 集群相关

1. 启动kafka

   `./kafka-server-start.sh config/server.properties &`

   ​


# kafka
Basic information for work with Apache Kafka

1. Install JDK11 and Zookeeper
    https://jdk.java.net
    https://zookeeper.apache.org/releases.html
```sh
    # tar -zxf zookeeper-3.4.6.tar.gz
    # mv zookeeper-3.4.6 /usr/local/zookeeper
    # mkdir -p /var/lib/zookeeper
    # cat > /usr/local/zookeeper/conf/zoo.cfg << EOF
    > tickTime=2000
    > dataDir=/var/lib/zookeeper
    > clientPort=2181
    > EOF
    # export JAVA_HOME=/usr/java/jdk1.11.0.10
    # /usr/local/zookeeper/bin/zkServer.sh start
    JMX enabled by default
    Using config: /usr/local/zookeeper/bin/../conf/zoo.cfg
    Starting zookeeper ... STARTED
    #
```
3. Configure zookeeper with /bin/zoo.cfg file. Example in the folder
4. Install Apache Kafka
    https://kafka.apache.org/downloads.html

```sh
  # tar -zxf kafka_2.13-2.7.0.tgz
  # mv kafka_2.13-2.7.0 /usr/local/kafka
  # mkdir /tmp/kafka-logs
  # export JAVA_HOME=/usr/java/jdk1.11.0.10
  # /usr/local/kafka/bin/kafka-server-start.sh -daemon
  /usr/local/kafka/config/server.properties
  #
```



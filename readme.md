Using Apache Kafka 0.11

tar -xzf kafka_2.11-0.11.0.0.tgz
cd kafka_2.11-0.11.0.0.tgz
./bin/zookeeper-server-start.sh config/zookeeper.properties


bin/kafka-console-producer.sh --broker-list localhost:9092 --topic test
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
 


mvn assembly:assembly

Start Consumer

java -cp target/kafka-example-0.0.1-SNAPSHOT.jar kafka.consumetConsumer 

Start Producer

java -jar target/kafka-example-0.0.1-SNAPSHOT.jar 


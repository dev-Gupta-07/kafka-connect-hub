
Commands for nodejs

docker run -p 2181:2181 zookeeper

docker run -p 9092:9092 \
-e KAFKA_ZOOKEEPER_CONNECT=192.168.29.176:2181 \
-e KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://192.168.29.176:9092 \
-e KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR=1 \
confluentinc/cp-kafka

{at place of it 192.168.29.176} replace with ip address of your zookeeper

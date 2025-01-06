# Kafka application deployment
To deploy Kafka to be used by a Python application.

```
docker compose up
```

## Create consumer/producer using command line
In case you want to create a consumer/producer using command line, you can follow these applications:

 - Create the producer:

```
docker exec -it kafka /bin/bash
kafka-console-producer.sh --broker-list localhost:9093 --topic test
```

 - Create the consumer:

```
docker exec -it kafka /bin/bash
kafka-console-consumer.sh --bootstrap-server localhost:9093 --topic test --from-beginning
```

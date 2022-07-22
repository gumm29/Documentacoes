# Kafka
## Instalação
### Linux:
Seguir o [tutorial](https://www.javatpoint.com/installing-kafka-on-linux)
### Rodar Kafka
Na pasta do kafka pelo terminal, abrir dois terminais, um para o zookeeper e outro para o servidor do kafka.
Rodar zookeeper:
>zookeeper-server-start.sh config/zookeeper.properties
Rodar kafka:
>kafka-server-start.sh config/server.properties
### Criar um topico e visualizar todos os topicos
>kafka-topics.sh --bootstrap-server localhost:9092 --topic text_topic --replication-factor 1 --partitions 1
Para ver os topicos:
>kafka-topics.sh --bootstrap-server localhost:9092 --list
### Enviar e receber uma mensagem (producer e consumer)
Abrir mais dois terminais, um para o producer e outro para o consumer
Producer:
>kafka-console-producer.sh --broker-list localhost:9092 --topic text_topic
Consumer:
>kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic text_topic --from-beginning

Ira abrir um console no producer e um no consumer
digite algo no producer e digite enter, vá para o consumer e a mensagem esta rá lá.

Obs:
*nome do topico criado text_topic
*porta 9092 - porta padrao do kafka

Explicacao de [kafka](https://www.youtube.com/watch?v=M4mHkuQ0mqQ)

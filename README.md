# Kafka + Hive + Presto + Minio + Polynote + Hue.

Utilizando `docker-compose` temos o Confluent Kafka, Presto, Hadoop, Minio, Polynote (Com Apache Spark), possibiltando o Presto fazer queries em dados no Minio e o Apache Spark ler arquivos do Minio. O presto utiliza o Hadoop como metastore.

# Executar o projeto 

Para executar o projeto digitar no terminal: 
```
docker-compose -f docker-compose-all-in-one.yml up -d
```
Confluent Kakfa:         http://localhost:9021/<br/>
Minio:                   http://localhost:9000/<br/>
Presto WebUI:            http://localhost:8080/<br/>
Polynote:                http://localhost:8192/<br/>
Hue:                     http://localhost:8888/<br/>

<br/>
Para executar somente o Confluent Kafka use:
```
docker-compose -f docker-compose-kafka.yml up -d
```
<br/>
Para executar Hive + Presto + Minio + Polynote + Hue use:
```
docker-compose up -d
```

# Encerrando o projeto

Para encerrar execute no terminal. 
```
docker-compose -f <arquivo> down
```
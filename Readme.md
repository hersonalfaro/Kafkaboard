Kafkaboard
==========

Simple kafka dashboard for following streamed messages by topic.

How to use?
===========

Run at project directory:

```
$ run main.go
```

After this application will start at "localhost:8080". As default, application listening local kafka port (localhost:9092)

Using different IP
===========

For different IP change helpers/KafkaHelper.go :

```go

conn, _ := kafka.DialLeader(context.Background(), "tcp", "YOUR_IP", topic, partition)

```
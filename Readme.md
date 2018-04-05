Kafkaboard
==========

Simple kafka dashboard for following streamed messages by topic.

![alt text](screenshots/screenshot.png "Kafkaboard")

How to use?
===========

Run at project directory:

```
$ go run main.go
```

After this application will start at "localhost:8080". As default, application listening local kafka port (localhost:9092)

## Using different IP

For different IP change helpers/KafkaHelper.go :

```go

conn, _ := kafka.DialLeader(context.Background(), "tcp", "YOUR_IP", topic, partition)

```

## Libraries used : 
- Beego (https://github.com/beego), 
- segmentio/kafka-go (https://github.com/segmentio/kafka-go)

## Dashboard template : 
- StarAdmin Free (https://github.com/BootstrapDash/StarAdmin-Free-Bootstrap-Admin-Template)


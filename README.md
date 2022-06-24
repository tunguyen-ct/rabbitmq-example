# Start RabbitMQ Docker Container

```
docker run -d --hostname my-rabbit --name some-rabbit -p 8080:15672 -p 5672:5672 rabbitmq:3-management
```

# Open RabbitMQ Dashboard

```
http://localhost:8080/
```

username: guest

password: guest


# Run Node.js Consumer

```
cd consumer
yarn install
node receive.js
```

# Run Golang Producer

```
cd producer
go mod tidy
go run send.go
```
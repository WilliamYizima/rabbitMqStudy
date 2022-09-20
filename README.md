# RabbitMQ

-> Content and tips taken from the book: RabbitMQ in Action: Distributed Messaging for Everyone

## Setup:
- [] Docker
- [] Docker-Compose
- [] Install python > Python2.7 

# Dev Enviroment
## Create a Image to RabbitMQ
```
docker build -t testemq --file dockerFileRabbitMq .
```

## Run container
```
docker run --name rabbit -p 5672:5672 -p 15672:15672 -d  testemq:latest
```

## See the RabbitMQ UI
```
http://localhost:15672/

user: guest
password: guest
```

## Add a new VHost:
- Go in tab 'Admin'
- In menu (right) choice 'VirtualHost'
- Click in 'Add a new virtual host'
- Input Name: dev-host
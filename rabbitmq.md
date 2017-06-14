# RabbitMQ

## Install on Ubuntu

`apt install rabbitmq-server`

## Start and stop
 
 `invoke-rc.d rabbitmq-server start`
 
 `invoke-rc.d rabbitmq-server stop`
 
 ## Connecting to RabbitMQ using Python
 
 ```python
 from librabbitmq import Connection
 conn = Connection()
 ```

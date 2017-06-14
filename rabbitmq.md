# RabbitMQ

## Installation

### Ubuntu

`apt install rabbitmq-server`

### Mac

`brew install rabbitmq`

## Start and stop
 
### Ubuntu

`invoke-rc.d rabbitmq-server start`

`invoke-rc.d rabbitmq-server stop`

### Mac

`brew services start rabbitmq`

`brew services stop rabbitmq`

 ## Connecting to RabbitMQ using Python
 
 ```python
 from librabbitmq import Connection
 conn = Connection()
 ```

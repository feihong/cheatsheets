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

## Web UI

http://localhost:15672/

## HTTP API

`curl -i -u guest:guest http://localhost:15672/api/vhosts`

## Config file location

Debian: `/etc/rabbitmq/rabbitmq.config`

Mac: `/usr/local/etc/rabbitmq/rabbitmq.config` (if installed via brew)

 ## Connecting to RabbitMQ using Python
 
 ```python
 from librabbitmq import Connection
 conn = Connection()
 ```

## Sources

- http://www.rabbitmq.com/configure.html#config-location

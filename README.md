
## Startup

`docker-compose up -d `

## Accessing Wordpress

The Wordpress site is available at localhost:8080.

http://localhost:8080/wp-login.php

## Accessing MySQL

docker exec -it <YOUR_SERVICE_NAME> bash


## Shutdown

To remove the container and default network, run:

`docker-compose down`

To also remove the database, run:

`docker-compose down --volumes`

## Hosting on Internet
Using ngrok you can expose your local docker wordpress instance to the internet.

ngrok http 8080 -host-header="localhost:8080"

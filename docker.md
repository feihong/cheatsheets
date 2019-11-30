# Docker

List images

    docker images
    
Remove image centos, including the containers that use it

    docker rmi -f centos

List running containers

    docker ps

List all containers, including paused ones

    docker ps -a

Remove all stopped containers, all dangling images, and all unused networks

    docker system prune

Build image with name 'ihaskell' and tag 'latest' using Dockerfile in current directory

    docker build -t ihaskell:latest .

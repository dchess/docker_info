# Intro to Docker
![](https://docs.docker.com/images/docker-docs-logo.svg)

## What is a Docker container?

* A lightweight way to package all the system dependencies for your code
* If you've ever used a virtual machine (VM) before, it's sort of like that
    but without the setup and is smaller and easier to share.
* It makes it so you can code once and deploy anywhere
* [Docker can explain this better than me](https://www.docker.com/resources/what-container)

## Why do I need them?

* Maybe you don't!
* But, if you are collaborating on code, deploying to environments different than where you develop,
    or just need to orchestrate a bunch of different applications/scripts then it might be a life-saver.
* One of the main benefits is that it solves the "It works on my machine" problem.
* It also make its easy to deploy to multiple environments (Mac, Linux, Windows) and easily 
    replicate configurations across deployments (test vs staging vs production, etc)

## How do I get started?

* [Install Docker Desktop](https://docs.docker.com/install/)
* [Create a DockerHub account](https://hub.docker.com/signup)
* Identify some potential use cases
* Identify the right container image for your needs

## What are some example use cases?

* Web apps --> kippgalaxy (data portal)
* Microservices (think ETL) --> PS to Illuminate Connector
* Local databases (for testing?) --> Test environment for SQL Server or Postgres

## Start building with Docker

* [Docker Pull](https://docs.docker.com/engine/reference/commandline/pull/)
* [Docker build](https://docs.docker.com/engine/reference/commandline/build/)
* [Docker Run](https://docs.docker.com/engine/reference/commandline/run/)
* Utility commands
    * `docker image ls`: list all docker images on your machine
    * `docker ps --all`: list all docker containers (running or not) on your machine
    * `docker system prune`: remove unused data such as stopped containers and incomplete builds

## Where can I learn more?

* [Docker Concepts Introduction](https://www.youtube.com/watch?v=6aBsjT5HoGY)
* [Docker Quick-Start Tutorial](https://docs.docker.com/get-started/)
* [Docker documentation](https://docs.docker.com/)
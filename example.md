# Docker Example

## Spin up MS SQL server in a Docker container

```bash
$ docker run -d --name mssql -p 1433:1433 -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=DataWhiz2019" mcr.microsoft.com/mssql/server:2017-latest-ubuntu
```

Stop your container

```
$ docker container stop mssql
```

Restart your container

```
$ docker container start mssql
```

Remove your container

```
$ docker containter rm mssql
```

Create a new image (but with a mapped volume: persistent storage)

```
$ docker run -d --name mssql -p 1433:1433 -v ${PWD}/data:/var/opt/mssql -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=DataWhiz2019" mcr.microsoft.com/mssql/server:2017-latest-ubuntu
```

## Start an interative shell inside your Docker container

```
$ docker exec -it mssql /opt/mssql-tools/bin/sqlcmd -S localhost -U sa -P DataWhiz2019
```

## Connect with SSMS or your Database IDE of choice

```
server=localhost
port=1433
user=sa
password=DataWhiz2019
```


## Next Steps

* Learn about [docker-compose](https://docs.docker.com/compose/)
* [Install docker-compose](https://docs.docker.com/compose/install/)
* [Explore DockerHub](https://hub.docker.com/search?q=&type=image)
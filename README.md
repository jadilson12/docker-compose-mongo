<p align="center">
   <img src="https://i.imgur.com/oCevKmo.png" width="500">
</p>

# Description

Docker using compose, configuration file with environment variables and creating a container,
in addition the data are present on the local machine even after restart or re created the container :

- mongodb:latest

# Mongodb Container Configuration

1. Expose port

   - 12017

2. Volume (Note: check if in the docker configuration -> shared drivers, the units are enabled)

   - Application database: ./docker/mongo/data -> /data/db

# How to use

1. Clone the repository using the command:

```
$ git clone https://github.com/jadilson12/docker-compose-mongo
```

2. Enter the folder docker-compose-mongo copy the files

```
$ cp env-example .env
$ cp docker-compose.yml-example docker-compose.yml
```

3. Run your container:

```
$ docker-compose up -d
```

4. Access the container shell:

```
$ docker exec -it app-database sh
```

## Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/jadilson12/docker-compose-mongo/issues).

## Show your support

Give a ⭐️ if this project helped you!

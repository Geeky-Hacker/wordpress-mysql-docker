# wordpress-mysql-docker

A local Wordpress instance using docker-compose. 

The project contains a `docker-compose` which configures a local Wordpress instanace with MySQL. 
It also has persistence unit so your changes won't get lost after stopping the containers.

- MySQL accessible via `localhost:3306` with `root` and `secret` credentials
- Wordpress accessible via `localhost`

## Start and stop

To start just run the docker-compose,

```bash
$ docker-compose up -d
```
To stop (but keeping the persisted data),

```bash
$ docker-compose down
```

To stop and remove data (volumes)

```bash
$ docker-compose down -v
```

## Important note

Do not use this set up for production. This is suitable for local testing only.

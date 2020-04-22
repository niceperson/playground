# Infra
For local dev traefik using traefik and some basic stuff like db and redis

# Tech
* A minimal setup just traefik.
* Basic Infra would be with DB and Redis

# Infra Setup
Duplicate `sample.env` into `.env`  and set the env-variable with appropriate value
Create volume run this command `docker volume create letsencrypt`

#### Note
We could also spin only the desired container for example

only traefik and redis
```sh
docker-compose up -d traefik redis
```
traefik redis and postgres
```sh
docker-compose up -d traefik redis postgres
```
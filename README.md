# Docker Compose Collections

Just a collection of [`docker-compose.yml`](https://docs.docker.com/compose/) for quick setup of your development. All of the them have a GUI option included for managing the data easier through browser. All of the data should be persistent (data is still there when restarting the container) except, well, memcached.

- Cache
  - [Redis](https://redis.io/) & [admin](https://github.com/joeferner/redis-commander)
  - [Memcached](https://memcached.org/) & [admin](https://github.com/elijaa/phpmemcachedadmin)
- Database
  - [MySQL](https://www.mysql.com/) & [admin](https://www.adminer.org/)
  - [PostgreSQL](https://www.postgresql.org/) & [admin](https://www.adminer.org/)
  - [MongoDB](https://www.mongodb.com/) & [admin](https://github.com/mongo-express/mongo-express)
- Pubsub
  - [RabbitMQ](https://www.rabbitmq.com/) & admin
  - [NSQ](https://nsq.io/) & admin
- Others
  - [Elasticsearch](https://www.elastic.co/) & [Kibana](https://www.elastic.co/kibana)

## Requirement

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Installation

1. Clone this repo.
    ```bash
    git clone https://github.com/rl404/docker-compose-collections.git
    ```
2. Go inside.
    ```bash
    cd docker-compose-collections
    ```
3. Modify the `yml` file that you want to build especially the `environment` part.
4. Build and run your desired rcontainers.
    ```bash
    docker-compose -f filename.yml up
    ```
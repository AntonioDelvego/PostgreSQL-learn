# PostgreSQL-learn
Learning PostgreSQL

Инструкция рассчитана на запуск приложения на ОС Linux 

Для запуска и работы приложения требуется установленные Docker и Docker Compose (standalone версия docker compose).

Для проверки правильности установки необходимо выполнить команды (команды выполнять без sudo и не под root):

```shell
docker --version

docker-compose --version

docker run hello-world 
```

Ожидаемый результат:

```shell
Docker version 20.10.18, build b40c2f6b5d
Docker Compose version 2.11.2
```
```shell
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
2db29710123e: Pull complete 
Digest: sha256:18a657d0cc1c7d0678a3fbea8b7eb4918bba25968d3e1b0adebfa71caddbc346
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/
```

## Установка
В папке с приложением выполните команду
```shell
./lde install
```

## Запуск
В папке с приложением выполните команду
```shell
./lde up
```

## Остановка
В папке с приложением выполните команду
```shell
./lde down
```

---
PGAdmin будет доступен по адресу http://localhost:<PG_ADMIN_PORT> (смотрите значение в .env), по умолчанию - http://localhost:8999

Имя пользователя в postgres - имя вашего пользователя в системе - `whoami`

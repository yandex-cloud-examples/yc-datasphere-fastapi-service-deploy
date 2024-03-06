# Развертывание сервиса в Yandex DataSphere на основе Docker-образа с FastAPI

Пример содержит простейший Docker-образ на основе фреймворка FastAPI для развертывания сервиса в Yandex DataSphere. Сервис предусматривает проверки работоспособности образа и отправляет метрики в формате Prometheus.

## Как собрать Docker-образ

Установите Docker. В командной оболочке выполните следующие команды:

```
docker build --platform linux/amd64 -t fastapi-docker .
docker tag fastapi-docker <docker_repo_with_tag>
docker push <docker_repo_with_tag>
```

Подробное руководство см. в [документации Yandex Cloud](cloud.yandex.ru/docs/datasphere/tutorials/node-from-docker-fast-api).
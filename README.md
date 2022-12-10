# Геосервер для чайников

Собраны минимально необходимые компоненты для развертывания геосервера с использованием контейнеров [Docker](https://www.docker.com/).

**Состав:**

- [GeoServer](https://geoserver.org/)
- [NGINX Proxy manager](https://nginxproxymanager.com/)
- [PostGIS](https://postgis.net/)
- [pgAdmin](https://www.pgadmin.org/)

## Реализация

Каждый проект содержит файлы `docker-compose.yml` и разворачивается через утилиту `docker-compose`.

Требования:

- установленный `docker` и `docker-compose`
- создана внутренняя сеть `docker network` (по умолчанию принято название `webgis`)

Данный репозиторий содержит ссылки на другие репозитории, поэтому клонировать командой:

```shell
git clone --recurse-submodules git@github.com:alexlipovka/glimmering_city.git
```

Либо последовательно вызвать:

```shell
git clone git@github.com:alexlipovka/glimmering_city.git
git submodule init
git submodule update
```

Кроме того, можно клонировать обычным образом и потом открывать проект в VS Code, чтобы видеть все содержимое без скачивания:

```shell
git clone git@github.com:alexlipovka/glimmering_city.git
cd glimmering_city
code .
```
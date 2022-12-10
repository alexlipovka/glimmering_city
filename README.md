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
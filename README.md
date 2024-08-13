# Ubuntu docker container.
## Описание:

## Просто linux для некоторых тестов, работа и то, что вам нужно сделать в linux.

## Примечание!
## Установите для вашего git следующую команду.

    git config --global core.autocrlf false

Because trailing characters ^M will affect the docker image build.

## Как использовать:
## Сборка образа docker.
docker build -t your_image_tag .
## Запуск контейнера с переадресацией 22 портов.
docker run -id --name container_name -p 22:22 your_image_tag
## Подключитесь к своему контейнеру:
docker exec -it container_name /bin/bash
## Или используйте ssh
login:root password:root

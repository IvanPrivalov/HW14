# Docker

## Задание
Создайте свой кастомный образ nginx на базе alpine. После запуска nginx должен отдавать кастомную страницу (достаточно изменить дефолтную страницу nginx)

Ссылка на Docker Hub (https://hub.docker.com/r/privalovip/nginx_alpine)

Для проверки задания выполнить:
```shell
docker run -d -p 80:80 --name nginx_alpine privalovip/nginx_alpine:0.1
```
Перейдите на страницу http://localhost/ в браузере.

## Ответы на вопросы

### Определите разницу между контейнером и образом.
Образ - это файл, включающий зависимости, сведения, конфигурацию для дальнейшего развертывания и инициализации контейнера. Контейнер - это работающий (выполняющийся) экземпляр образа, который включает в себя все необходимое для запуска внутри какго-либо приложения (код приложения, среду выполнения, библиотеки, настройки и т.д), из одного образа можно создать неограниченное количество контейнеров.

### Можно ли в контейнере собрать ядро?
Да, можно, как и любую программу из исходников.

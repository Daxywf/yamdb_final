# api_yamdb
REST api для проекта YaMDb - базы с отзывами о различных произведениях.

## Описание
Позволяет работать со следующими объектами:
- Пользователи
- Отзывы
- Комментарии к отзывам
- JWT - токен
- Категории
- Жанры
- Произведения

Полная докуметрация проекта с примерами запросов к api: [redoc.yaml](https://github.com/Daxywf/api_yamdb/blob/master/api_yamdb/static/redoc.yaml)

## Как запустить проект (docker)
- Скачать docker с [официального сайта](https://www.docker.com/products/docker-desktop) и установить его.
- Клонировать репозиторий с проектом и перейти в него 
```git clone https://github.com/Daxywf/infra_sp2``` ```cd infra_sp2```
- Запустить docker-compose из соответствующей директории
```cd infra ``` ```docker-compose up```

При первом запуске
- Выполнить миграции
```docker-compose exec web python manage.py migrate```
- При желании загрузить в базу демо-данные
```docker-compose exec web python manage.py loaddata fixtures.json```

## Участники

Александр Страхов

Дмитрий Деев

Владимир Сергеев

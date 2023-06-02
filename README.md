URL
Проект развернут на сайте: https://kittygram47.ddns.net/signin

Описание
Интерактивный сайт с личным кабинетом с возможностями публикации фотографий котов, а также присваивания достижений.

Технологии
Python 3.11.1, Django 4.1, Django REST framework, React

Запуск проекта в dev-режиме

Клонируйте репозиторий и перейдите в него в командной строке:
git clone https://github.com/AleksandrPerepelkin/kittygram_final.git

cd kittygram_final

Запустите проект с помощью команды:

docker compose up

Соберите статику Django с помощью команды:
docker compose exec backend python manage.py collectstatic

Скопируйте статику командой:
docker compose exec backend cp -r /app/collected_static/. /static/static/

По адресу http://127.0.0.1:9000/ сайт будет доступен.

Автор
Perepelkin Aleksandr

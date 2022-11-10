# ChillnoWork
Лучший сервис на фастапи для путешесьвенников
1. Запуск docker-compose:

$ sudo docker-compose up

2. Настройка БД:

$ sudo  docker exec -ti chillnowork_postgres_1 /bin/sh
$ psql -U myuser
$ ALTER ROLE myuser WITH PASSWORD '1234';
$ CREATE DATABASE fastapi_database;

3. Если все ок то выходим из psql и запускаем alembic( уже с готовыми миграциями)

$ alembic upgrade head
4.Настройка nginx

# Yamdb
## База отзывов пользователей о фильмах, музыке и книгах
## Стек технологий: Python 3, Django REST Framework, PostgreSQL, Simple-JWT, NGINX, Docker

### Запуск приложения:
``` git clone https://github.com/Lev1sDev/infra_sp2.git  ``` \
```docker-compose up```

### Выполнить миграции:
```docker-compose exec web python manage.py makemigrations``` \
```docker-compose exec web python manage.py migrate --noinput```

### Создать суперпользователя:
```docker-compose exec web python manage.py createsuperuser```

### Привязать статические файлы:
```docker-compose exec web python manage.py collectstatic --no-input```

### Заполнить базу начальными данными:
```docker-compose exec web python manage.py loaddata fixtures.json```
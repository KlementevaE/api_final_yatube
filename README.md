# api_final

### Описание

API социальной сети для публикации личных дневников. Можно создавать свои посты, комментировать их и подписываться на других авторов.

### Технологии

- Python 3.8.10
- Django 2.2.16
- Django REST Framework 3.12.4
- Simple-JWT

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/KlementevaE/api_final_yatube.git
```

```
cd api_final_yatube

```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
cd yatube_api
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```
### Примеры запросов к API:
```
GET:
http://127.0.0.1:8000/api/v1/posts/
[
    {
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
    }
]
GET:
http://127.0.0.1:8000/api/v1/groups/
[
  {
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
  }
]
```
### Автор

Клементьева Евгения

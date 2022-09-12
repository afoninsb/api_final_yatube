
# yatube_api

Блогоплатформа, построенная на API


## Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:afoninsb/api_final_yatube.git
```

```
cd yatube_api
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
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```
## Примеры запросов

GET http://127.0.0.1:8000/api/v1/posts/
Ответ:
{
  "count": 123,
  "next": "http://api.example.org/accounts/?offset=400&limit=100",
  "previous": "http://api.example.org/accounts/?offset=200&limit=100",
  "results": [
    {
      "id": 0,
      "author": "string",
      "text": "string",
      "pub_date": "2021-10-14T20:41:29.648Z",
      "image": "string",
      "group": 0
    }
  ]
}

POST http://127.0.0.1:8000/api/v1/posts/
Payload:
{
  "text": "string",
  "image": "string",
  "group": 0
}

## 🚀 Документация API
http://127.0.0.1:8000/redoc/


## 🚀 About Me
I'm a backend-developer...


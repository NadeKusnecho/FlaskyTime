# Quick Start

## Windows

### Создание виртуального окружения

```
pip install virtualenv
virtualenv venv
venv\Scripts\activate
```

### Установка зависимостей

```
pip install -r requirements.txt
```

### Добавление переменной окружения и режим отладки

```
set FLASK_APP=flasky.py
set FLASK_DEBUG=1
```

### Регистрация SMTP и почта администратора

```
set MAIL_USERNAME=nadekusnecho@gmail.com
set MAIL_PASSWORD=12345QAZqaz
set FLASKY_ADMIN=nadekusnecho@gmail.com
```

### Работа с базой данных

```
flask db init
flask db migrate
flask db upgrade
```

### Тестирование и запуск приложения

```
flask test
flask run
```

### API

```
http --json --auth nadekusnecho@gmail.com:12345 GET http://127.0.0.1:5000/api/v1/posts/
http --auth nadekusnecho@gmail.com:12345 --json POST http://127.0.0.1:5000/api/v1/posts/ "body=I'm adding a post from the *command line*.
http --auth nadekusnecho@gmail.com:12345 --json POST http://127.0.0.1:5000/api/v1/tokens/
http --json --auth eyJhbGciOiJIUzUxMiIsImlhdCI6MTYyNDQ0NDk0NywiZXhwIjoxNjI0NDQ4NTQ3fQ.eyJpZCI6MX0.RI95eYaVsQn6SK_OUazmGeSysfbcod_WHeqUhVj50lRF9ZpQIKc2facTMs07Hgxku8aaIfTJIRO5VdU7UQt5qw: GET http://127.0.0.1:5000/api/v1/posts
```

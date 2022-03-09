# Регистрация и авторизация пользователя

## Условия

### В проекте используется:

+ Python 3.9
+ Django 4.0.3
+ Django Rest Framework 3.13.1
### Установка необходимых пакетов:
```
pip install -r requirements.txt
```
### Затем выполнить миграцию:
```
python manage.py migrate
```
### После завершения миграции запустите сервер разработки с помощью команды:
```
python manage.py runserver
```
### Сервер работает по адресу http://localhost:8000

# Конечная точка API
### Регистрация:
```
/users/register/

Method:
POST

Headers:
Content-Type: application/json

Body:
{
    "username": "user",
    "password": "pass",
    "email": "email@mail.com"
}
```
### Авторизация:
```
/users/login/

Method:
POST

Headers:
Content-Type: application/json

Body:
{
    "username": "user",
    "password": "pass"
}
```
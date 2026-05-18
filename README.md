[![Main Kittygram workflow](https://github.com/Outsider133/kittygram_final/actions/workflows/main.yml/badge.svg?event=push)](https://github.com/Outsider133/kittygram_final/actions/workflows/main.yml)



# Kittygram

Kittygram - это сайт на котором люди могут делиться своими котами, фото, достижения, год рождения и клички, 
единственное правило - НИКАКИХ СОБАК!!!!

## Стек технологий

- Django
- Django rest API
- Docker
- Nginix
- pytest


##  Как работать с репозиторием финального задания

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram_backend.git
```

```
cd kittygram_backend
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

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


## Необходимые переменные для env файла


- POSTGRES_DB
- POSTGRES_PASSWORD
- POSTGRES_USER
- DB_NAME
- DB_HOST
- DB_PORT
- SECRET_KEY
- DEBUG
- ALLOWED_HOSTS


## Как проверить работу с помощью автотестов

В корне репозитория создайте файл tests.yml со следующим содержимым:
```yaml
repo_owner: ваш_логин_на_гитхабе
kittygram_domain: полная ссылка (https://доменное_имя) на ваш проект Kittygram
taski_domain: полная ссылка (https://доменное_имя) на ваш проект Taski
dockerhub_username: ваш_логин_на_докерхабе
```

Скопируйте содержимое файла `.github/workflows/main.yml` в файл `kittygram_workflow.yml` в корневой директории проекта.

Для локального запуска тестов создайте виртуальное окружение, установите в него зависимости из backend/requirements.txt и запустите в корневой директории проекта `pytest`.


## Автор: Кирилл Аристов
https://github.com/Outsider133

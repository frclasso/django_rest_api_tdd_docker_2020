# Django RestFramework API with TDD , Docker and Travis-CI


Faça download do projeto
------------------------


Rodando via docker
------------------
```
$ docker-compose up -d --build
$ docker-compose run app sh -c "python manage.py createsuperuser"
$ docker-compose run app sh -c "python manage.py makemigrations"
$ docker-compose run app sh -c "python manage.py migrate"
```


End points
----------

-----

JSON Data Payloads
------------------
- Para inserir dados utilizar o arquivo localizado em app/postman_collection
---

Testando
--------
``$ docker-compose run app sh -c "python manage.py test && flake8"
```
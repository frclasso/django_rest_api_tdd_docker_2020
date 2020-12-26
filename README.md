# Django RestFramework API with TDD , Docker and Travis-CI


Faça download do projeto
------------------------
    https://github.com/frclasso/django_rest_tdd_dockerdvanced.git

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
-http://localhost:8000/api/user/create/
-http://localhost:8000/api/user/token/
-http://localhost:8000/api/user/me/

-http://localhost:8000/api/recipe/ingredients/
-http://localhost:8000/api/recipe/tags/
-http://localhost:8000/api/recipe/recipes/

-----

JSON Data Payloads
------------------
- Para inserir dados utilizar o arquivo localizado em app/postman_collection
---

Testando
--------
```
$ docker-compose run app sh -c "python manage.py test && flake8"
```
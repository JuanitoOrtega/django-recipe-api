Todos los comandos python se ejecutan de la siguiente forma

```shell
docker-compose run --rm app sh -c "python manage.py collectstatic"
```

# Docker
-- Despues de crear el archivo Dockerfile
-- Creamos la carpeta app
-- Creamos nuestra imagen con el siguiente comando:

```shell
docker build .
```

### Creamos nuestro archivo docker-compose.yml

-- Ejecutamos el siguiente comando:

```shell
docker-compose build
```

### Para ejecutar pruebas en nuestro proyecto django

-- Ejecutamos el siguiente comando:

```shell
docker-compose run --rm app sh -c "python manage.py test"
```

### flake8
-- Ejecutamos el siguiente comando

```shell
docker-compose run --rm app sh -c "flake8"
```

### Django
-- Ejecutamos el siguiente comando para crear proyecto:

```shell
docker-compose run --rm app sh -c "django-admin startproject app ."
```

#### Lanzar proyecto o despues de edigar docker-compose.yml
```shell
docker-compose up
```
-- Ejecutar migraciones:

```shell
docker-compose run --rm app sh -c "python manage.py migrate"
```
-- Crear super usuario:

```shell
docker-compose run --rm app sh -c "python manage.py createsuperuser"
```

-- Ejecutar test:

```shell
docker-compose run --rm app sh -c "python manage.py test"
```

-- Crear app:

```shell
docker-compose run --rm app sh -c "python manage.py startapp core"
```
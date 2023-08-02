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

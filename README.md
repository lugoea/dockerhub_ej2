## dockerhub\_ej2

Con los pasos a continuación se realiza la descarga de una imagen existente y luego se sube a un repo de DockerHub.

*   Ejecutar el siguiente comando

```plaintext
docker pull nicopaez/pingapp:3.0.0
```

*   Crear repositorio en dockerhub usando la url 

[https://hub.docker.com/repository/create?namespace=elugo](https://hub.docker.com/repository/create?namespace=elugo)

*   Aplicar tag a la imagen descargada 

```plaintext
docker tag nicopaez/pingapp:3.0.0 elugo/taller-docker-ejercicio2:1.0.0
```

*   Subir la nueva imagen a Dockerhub

```plaintext
docker push elugo/taller-docker-ejercicio2:1.0.0
```

Luego de eso la imagen esta publicada y puede ser compartida a traves de DockerHub usando el comando

```plaintext
docker pull elugo/taller-docker-ejercicio2

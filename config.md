## Herramientas a usar:
* Docker
* Jenkins

1. Instalamos Docker
* Para Linux:

```bash
sudo apt-get update && apt-get install docker-ce docker-ce-cli containerd.io
```
* Para Windows/MacOS:

    - Ingresamos a la ruta [aquí](https://www.docker.com/products/docker-desktop), lo cual descargará Docker para escritorio.

2. En esta ocación vamos a instalar Jenkins mediante Docker, para ello ejecutamos el siguiente comando:
```bash
docker run -d -v <ruta_local>:/var/jenkins_home -p 8080:8080 -p 50000:50000 --name myjenkins jenkins/jenkins
```
3. Luego de arrancar el contenedor abrir un navegador y colocar lo siguiente:
```url
http://localhost:8080
```

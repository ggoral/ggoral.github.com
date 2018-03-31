---
layout: post
title:  "Instalación de Docker"
date:   2018-03-10 13:00:00 -0300
categories: docker
lang: es
ref: 2018-03-10-docker-get-started
---

## Instalación

El primer paso posterior despues de leer la introducción debería ser instalar correctamente docker, podemos seguir los pasos de la [Documentación Oficial][install-docker]

* Docker puede ser instalado sobre Linux, Windows, y Mac.

## Ambiente

Los primeros comandos que ejecutaremos describirán el estado de nuestro ambiente.

### Versión de Docker
{% highlight bash %}
$ docker --version
Docker version 17.12.1-ce, build 7390fc6
{% endhighlight %}

### Informacion del ambiente
{% highlight bash %}
$ docker info
Containers: 0
 Running: 0
 Paused: 0
 Stopped: 0
Images: 0
...
{% endhighlight %}

### Verificación de la instalación
Probamos que la instalación de docker este corriendo la imagen: **hello-world**
{% highlight bash %}
$ docker run hello-world
{% endhighlight %}

[install-docker]: https://docs.docker.com/install/

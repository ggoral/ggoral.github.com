---
layout: post
title:  "Introducción a Docker"
date:   2018-03-06 20:47:52 -0300
categories: devops docker
lang: es
ref: 2018-03-07-docker-introduction
---

## Resumen

Después de leer infinidad de sitios relacionados con Docker calificar algunos de ellos con algún criterio simple da como resultado un numero finito de ellos.
La versión oficial es siempre la mejor, en este caso la documentación oficial es muy buena pero comprende muchos documentos esto implica una inversión de tiempo significativa.

## Introducción

Suponiendo que el lector tiene un conocimiento previo sobre "[Que es Docker?][what-docker]", repasaremos dos conceptos importantes que debemos tener en cuenta:

1. Contenedor
2. Imagen

La *Imagen* es el molde de nuestro sistema operativo, la cual sera ejecutada.
El *Contenedor* sera la instancia de una imagen.

## Comandos Basicos
{% highlight bash %}
$ echo 'hola' >> /dev/null
{% endhighlight %}

[what-docker]: https://www.docker.com/what-docker

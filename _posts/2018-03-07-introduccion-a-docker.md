---
layout: post
title:  "Introducción a Docker"
date:   2018-03-07 20:47:52 -0300
categories: devops docker
lang: es
ref: 2018-03-07-docker-introduction
---

## Resumen

Después de leer infinidad de sitios relacionados con Docker calificar algunos de ellos con algún criterio simple da como resultado un numero finito de ellos.
La versión oficial es siempre la mejor, en este caso la documentación oficial es muy buena pero comprende muchos documentos esto implica una inversión de tiempo significativa.


### Antecedentes

Antiguamente, transportar bienes(aplicaciones) tenía muchos problemas:

* Diferentes tamaños, formas, resistencias, etc.
* Capacidad de transporte reducida.
* Difícil realizar un seguimiento.
* Pérdida parcial de mercadería(información).
* Grandes costos.

## Introducción

Suponiendo que el lector tiene un conocimiento previo sobre [Que es Docker?][what-docker], repasaremos tres conceptos importantes que debemos tener en cuenta: Docker, Imagen, y Contenedor

### ¿Que es Docker?

Es una aplicación para administrar contenedores de software. Docker empaqueta aplicaciones en una unidad estándar de intercambio.

Empaqueta todo el sistema operativo en un filesystem que contiene todo lo necesario para ejecutar una aplicación: código, librerías, herramientas, etc.

Garantiza que el software siempre correrá de igual forma sin importar su ambiente.


### ¿Que es una Imagen?
La imagen es el molde de nuestro sistema operativo, la cual sera ejecutada.

* Filesystem y parámetros para utilizarla.
* No cambia nunca y no tiene estados.

### ¿Que es un Contenedor?
El contenedor es la instancia de una imagen.

* Tiene una capa de escritura volátil.
* Por lo tanto al ejecutar una imagen tendremos un contenedor con nuestro sistema operativo corriendo.


## Beneficios de Docker
* Rápida configuración de entornos de desarrollo.
* Favorece las arquitecturas de microservicios.
* Diferencias entre el ambiente de desarrollo, testing y producción.
* Instalación de una aplicación en diferentes plataformas.
* Deploy de aplicaciones complejas.
* Ejecución de código antiguo.
* Escalamiento horizontal.




[what-docker]: https://www.docker.com/what-docker
[install-docker]: https://docs.docker.com/install/

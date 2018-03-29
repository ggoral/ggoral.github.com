---
layout: post
title:  "Primeros pasos en Python"
date:   2018-03-29 12:12:25 -0300
categories: python
lang: es
ref: 2018-03-29-python-get-started
---

## Instalación

Al igual que en otros manuales el primer paso luego de una breve introducción es instalar correctamente el ambiente. La recomendación es siempre la misma, ir a la [documentación oficial][python-oficial],

* Python puede ser instalado sobre muchos sistemas operativos Linux, Mac y Windows.

Este manual instalara Python en Ubuntu 16.04 queda a ejercicio del lector instalarlo en su sistema operativo.

## Instalando Python en Ubuntu 16.04

{% highlight bash %}
$ sudo apt-get update
$ sudo apt-get -y upgrade
$ sudo apt-get install -y python3-pip
$ sudo apt-get install build-essential libssl-dev libffi-dev python-dev
{% endhighlight %}


## Ambiente y versiones

El primer obstáculo que encontraremos al utilizar python es que la mayoría de los sistemas operativos viene con una versión desactualizada.


### Virtual Environment "venv"

Los "ambientes virtuales" te permiten tener un espacio aislado en tu computadora para los proyectos en python, asegurando que cada uno de los proyectos pueda tener su propio conjunto de dependencias y que estas no interfieran con otros proyectos.

Configurando el ambiente de programación nos provee un mejor control sobre nuestros proyectos, diferentes proyectos pueden tener diferentes dependencias, la convivencia de la mismas puede generar interferencias en diferentes proyectos.

Podemos configurar tantos ambientes de programacion como queramos. Cada ambiente es basicamente un directorio en tu computadora que tiene unos **scripts** y estos actuan como un ambiente.

Primero necesitamos instalar el modulo **venv** , que es parte de la libreria del Python 3, con esto podremos crear nuestros ambientes virtuales:

### Instalando venv en Ubuntu 16.04
{% highlight bash %}
$ sudo apt-get install -y python3-venv
{% endhighlight %}

Con **venv** instalado, seremos capaces de crear nuestros ambientes. Elegimos un directorio donde pondremos el ambiente.

{% highlight bash %}
$ mkdir environments
$ cd environments
{% endhighlight %}

Una vez en el directorio, creamos el ambiente con el siguiente comando:

{% highlight bash %}
$ python3 -m venv my_env
{% endhighlight %}

Esencialmente, esto configura un nuevo directorio el cual contiene unos archivos los cuales podemos ver con el comando **ls** :

{% highlight bash %}
$ ls my_env/
bin  include  lib  lib64  pyvenv.cfg  share
{% endhighlight %}

Para usar este ambiente, necesitamos activarlo, el cual podemos hacer escribiendo el siguiente comando:

{% highlight bash %}
$ source my_env/bin/activate
{% endhighlight %}

Para desactivar el ambiente simplemente escribiremos:

{% highlight bash %}
$ deactivate
{% endhighlight %}


## Probando el ambiente

Para probar el ambiente primero verificamos la versión de Python que tenemos instalado, como segundo paso activaremos el ambiente, crearemos un script del Python y verificamos la versión en la que se ejecuto.

### 1. Versión de Python
{% highlight bash %}
$ python --version
Python 2.7.12
{% endhighlight %}

### 2. Activaremos el ambiente
{% highlight bash %}
$ source my_env/bin/activate
{% endhighlight %}

### 3. Creamos un pequeño script para verificar la versión.
{% highlight bash %}
$ vi hello-world.py
{% endhighlight %}

En el script llamado hello-world.py escribiremos:
{% highlight python %}
#!/usr/bin/env python
# -*- coding: utf-8 -*-

import sys
print(sys.version)
{% endhighlight %}

Daremos permisos de ejecucion al script, y ejecutamos:
{% highlight bash %}
$ chmod +x hello-world.py
$ ./hello-world.py
3.5.2 (default, Nov 23 2017, 16:37:01)
[GCC 5.4.0 20160609]
{% endhighlight %}

## Conclusiones

En este punto tenemos instalado Python 3 como ambiente de programación para tu maquina con Ubuntu, ahora puedes empezar a escribir código en tu proyecto.

## Referencias y agradecimientos a:

* [Documentación Oficial][python-oficial]
* [Comunidad Python Argentina][python-argentina]
* [Digital Ocean por su excelente tutorial][install-python-digitalocean]

[python-oficial]: https://www.python.org/
[python-argentina]: http://www.python.org.ar/

[install-python-digitalocean]: https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04

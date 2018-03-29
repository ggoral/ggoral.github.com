---
layout: post
title:  "Tipos de Datos"
date:   2018-03-29 15:56:30 -0300
categories: python
lang: es
ref: 2018-03-29-data-types
---

## Variables

Las variables son contenedores de datos, en ellas se almacena el valor de algun tipo de dato que el lenguaje soporte. Pueden ser utilizadas para referenciar a otras variables ó a estructuras mas complejas.

* El nombre de las variables puede contener dígitos, letras y símbolo, pero deben comenzar con una letra.
* Las variables son *case sensitive*.
* Por convención se utilizara *snake_case* para nombres compuestos.

{% highlight python %}
a=b=c=1
print (a, b, c)
1 1 1

x, y, z = 3, 5, 7
print (x, y, z)
3 5 7

nombre_compuesto= "un nombre"
{% endhighlight %}


## Estilo de codificación
"El código es leído muchas más veces de lo que es escrito" Guido Van Roussen
* "La legibilidad cuenta" [PEP20][PEP0020]
* La guía de estilo para código Python es la [PEP08][PEP0008]

## Tipos de datos básicos

Dentro los tipos de datos básicos encontraremos tres grupos.

* Númericos
* * Enteros
* * Flotantes
* * Complejos
* * Octales
* * Hexadecimales
* Booleanos
* Cadenas de caracteres

### Númericos

Dentro de los tipos de datos númericos encontraremos los enteros, los flotantes y complejos. También tendremos a los octales y a los hexadecimales.

[PEP0008]: https://www.python.org/dev/peps/pep-0008/
[PEP0020]: https://www.python.org/dev/peps/pep-0020/

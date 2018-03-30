---
layout: post
title:  "Tipos de Datos Básicos"
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

nombre_compuesto = "un nombre"
{% endhighlight %}


## Estilo de codificación
"El código es leído muchas más veces de lo que es escrito" Guido Van Roussen
* "La legibilidad cuenta" [PEP20][PEP0020]
* La guía de estilo para código Python es la [PEP08][PEP0008]

## Tipos de datos básicos

Dentro los tipos de datos básicos encontraremos tres grupos.

* Númericos
* * Enteros
* * Reales
* * Complejos
* * Octales
* * Hexadecimales
* Booleanos
* Cadenas de caracteres

### Númericos

Dentro de los tipos de datos númericos encontraremos los enteros, los flotantes y complejos.

#### Enteros
* Un enteros se declaran directamente con un numero
* Un octal, anteponiendo un 0o (cero y letra o) o.
* Un hexadecimal, anteponiendo un 0x.

{% highlight python %}
var_entero = 2147483647
var_octal = 0o27
var_hex = 0x17
{% endhighlight %}

#### Reales
Se representan mediante los tipos float

{% highlight python %}
var_real1= 0.2703
var_real2= 0.1e-3
{% endhighlight %}

#### Complejos
Los numeros complejos se representa con el tipo de datos complex

{% highlight python %}
c1 = 4 + 3j
c1
c2 = complex(2, -3)
c2
type(c2)
complex
{% endhighlight %}

# https://relopezbriega.github.io/blog/2015/10/12/numeros-complejos-con-python/


[PEP0008]: https://www.python.org/dev/peps/pep-0008/
[PEP0020]: https://www.python.org/dev/peps/pep-0020/

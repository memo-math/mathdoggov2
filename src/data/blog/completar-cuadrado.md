---
author: MathDoggo
pubDatetime: 2026-05-12T17:00:00.000Z
modDatetime: 2026-05-12T17:00:00.000Z
title: Toolbox I. Completar el cuadrado
slug: completar el cuadrado
featured: true
draft: false
tags:
  - Algebra
  - Ecuacion Cuadratica
  - Matematicas Pre-Universitarias
  - Completar Cuadrado
  - Formula General
description: Post para comprender cómo completar el cuadrado y su importancia para resolver problemas e incluso deducir una fórmula.
---

Completar el cuadrado es una técnica de álgebra básica. Su objetivo es transformar una expresión de la forma
$ax^2 +bx +c$ en otra expresión equivalente de la forma $a(x+h)^{2}+k$. A primera vista, esta transformación parece ser artificial. Sin embargo, es una herramienta fuindamental que nos permite desde resolver ecuaciones cuadráticas hasta simplificar integrales o deducir la famosa fórmula general. 

## Procedimiento
La mejor manera de aprender la técnica es resolviendo un problema concreto.

Supongamos que queremos resolver la ecuación:

$$x^2+6x+5=0$$

En un primer paso pasemos el término constante del otro lado:

$$x^2+6x=-5$$

Ahora nuestro objetivo es convertir el lado izquierdo en un cuadrado perfecto, para esto tomamos el coeficiente
del término lineal, lo dividimos entre dos y lo elevamos al cuadrado:

$$ (\frac{6}{2})^2=9 $$

Sumamos este término en ambos lados de la ecuación para mantener la igualdad:

$$x^2 + 6x + 9 = -5 + 9$$

Lo importante aquí es notar que el lado izquierdo es ahora un trinomio cuadrado perfecto. Ahora podemos
factorizar:

$$(x+3)^2=4$$

Tomando raíz cuadrada en ambos lados tenemos:

$$ x + 3 = \pm 2$$

Así concluimos que $x=-1$ ó $x=-5$. 

Como podemos observar lo que tenemos que hacer para poder completar el 
cuadrado es sumar y restar el coeficiente del término lineal dividido entre dos y elevado al cuadrado.

En este momento es natural que nos preguntemos: ¿Qué pasa con una ecuación cuadrática más general, es decir, una cuyo coeficiente para el término cuadrático $(x^2)$ no sea $1$? Por ejemplo, supongamos que queremos resolver la ecuación $2x^2 + 8x + 6 = 0$. El procedimiento es casi el mismo, simplemente debemos dividir ambos lados de la ecuación por el coeficiente
del término cuadrático:

$$ \frac{2x^2+8x+6}{2} = \frac{0}{2} $$

$$ x^2 + 4x + 3 = 0 $$

De aquí el procedimiento es el mismo. Así que a partir de ahora cuentas con una herramienta para 
resolver ecuaciones cuadráticas, aunque a veces no sea el método más rápido.

## Deduciendo la fórmula general.

La famosa fórmula general, la chicharronera, no salió de la nada. De hecho es el resultado de resolver la ecuación cuadrática $ax^2 +bx +c=0$. Y en este pequeño post vamos a ver cómo sale esta fórmula. 

Partimos de la ecuación:

$$ ax^2+bx+c=0, a\neq 0$$

Dividimos entre $a$ y movemos el término constante:

$$ x^2 + \frac{b}{a}x =  -\frac{c}{a} $$

Ahora completamos el cuadrado sumando de ambos lados de la ecuación $(b/2a)^2$:

$$x^2 + \frac{b}{a}x + (\frac{b}{2a})^2 = - \frac{c}{a} + (\frac{b}{2a})^2$$

Por lo anterior sabemos que podemos factorizar fácilmente el lado izquierdo y haciendo un poco de álgebra y efectuando suma de fracciones del lado derecho llegamos a que: 

$$ (x+\frac{b}{2a})^2 = \frac{b^2-4ac}{4a^2} $$

Tomando raíz cuadrada:

$$ x + \frac{b}{2a} = \pm \frac{\sqrt{b^2 - 4ac}}{2a}$$

Despejando x obtenemos:

$$ x=\frac{-b \pm \sqrt{b^2-4ac}}{2a} $$

Y hemos logrado deducir la fórmula general!!!!

## Aplicaciones en la Geometría Analítica

Ya hemos mencionado que la técnica que estamos estudiando tiene utilidad en distintas clases de problemas por lo que veámosla en acción.

- Dada la circunferencia de ecuación $x^2 + y^2 - 2x + 4y - 4 = 0$. Hallar el centro y el radio.

Sol. Primero acomodamos la ecuación para que tengamos algo como esto:

$$ (x^2 - 2x) + (y^2 + 4y) = 4 $$

Ahora completamos el cuadrado para $x$ y para $y$ de forma independiente:

$$ (x^2 - 2x + 1) + (y^2 + 4y + 4) = 4 + 1 + 4$$

Factorizamos los trinomios cuadrados perfectos:

$$ (x-1)^2 + (y+2)^2 = 9 $$

Y con un poco de conocimientos en esta área sabemos que en esta forma la ecuación nos dice que el centro y el radio son

$$ C(1, -2) \text{ y } r=3$$

## Aplicaciones en Cálculo

- Resuelve la siguiente integral:

$$ \int \frac{dx}{x^2+10x+26} $$

Sol. Como puedes intuir por la temática del post que estás leyendo este problema se soluciona completando el cuadrado en el denominador. 

Observamos que la transformación que aplicamos al coeficiente del término lineal es:

$$ (\frac{10}{2})^2 = 25 $$

Entonces lo que necesitamos para completar el cuadrado es un $25$ pero este lo podemos sacar del término independiente del denominador $26 = 25 + 1$. Por lo que tendríamos 

$$ \int \frac{dx}{x^2+10x+26} = \int \frac{dx}{x^2+10x+25+1} =  \int \frac{dx}{(x+5)^2+1}$$

Ahora hacemos un cambio de variable $u = x+5$ entonces $du=dx$ y podemos reescribir la integral

$$ \int \frac{dx}{u^2+1} $$

Y normalmente es aquí donde podemos parar y ver que podemos reconocer la forma de la integral y ver que su antiderivada es la función arcotangente, esto con la ayuda de un formulario en caso de ser necesario. Entonces tenemos que el resultado de la integral ya con todo y volviendo a la variable original es:

$$ arctan(x+5) + C $$
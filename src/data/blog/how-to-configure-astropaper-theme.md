---
author: MathDoggo
pubDatetime: 2026-01-10T13:04:53.851Z
modDatetime: 2026-01-10T13:04:53.851Z
title: Aplicando la Propiedad Arquimediana
slug: Aplicando la Propiedad Arquimediana
featured: true
draft: false
tags:
  - Analisis Real
  - Calculo
  - Matematicas Universitarias
  - Propiedad Arquimediana
description: Ejemplo de cómo usar la Propiedad Arquimediana para resolver problemas de Análisis Matemático
---

La propiedad Arquimediana es una característica fundamental de los números reales y es uno de esos conceptos que aparecen muy pronto en los cursos de Análisis Matemático. El objetivo de este post es ayudar a los estudiantes o entusiastas que se enfrentan a este concepto por primera vez, ejemplificando su uso para resolver problemas. En este caso, he seleccionado dos ejercicios del libro de Understanding Analysis de Abbot.

Lo primero que hacer es enunciar la formulación de la propiedad arquimediana que nos da el libro antes citado.

Propiedad Arquimediana.
- Dado cualquier número $x\in \mathbb{R}$, existe un $n\in N$ que satisface que $n > x$.
- Dado cualquier número real $y > 0$, existe $n\in N$ que satisface que $\frac{1}{n} < y$
Ahora sí podemos pasar a los problemas.

**Primer problema**. Utiliza la propiedad Arquimediana de $\mathbb{R}$ para demostrar que 

$$\text{inf}\{1/n:n\in\mathbb{N}\}=0$$.

Demostración. Para mostrar que $0$ es un ínfimo debemos verificar que:

- $0$ es una cota inferior y
- $0$ es la máxima cota inferior.

Como $n\in \mathbb{N}$ es claro que $0\leq\frac{1}{n}$ para todo $n$. Por lo que $0$ es una cota inferior. Ahora queremos ver que si $x$ es una cota inferior, entonces $x\leq 0$. Por contradicción supongamos que $x > 0$ es cota inferior. Entonces por la propiedad Arquimediana existe $n_0\in\mathbb{N}$ tal que 
$1/n_{0}< x$. Pero $1/n_{0}\in \{1/n:n\in\mathbb{N}\}$. Entonces $x$ no es una cota inferior. Hemos llegado a una contradicción. Por lo que $x\leq 0$. Que es lo que queríamos demostrar.

**Segundo Problema**. Demostrar que 
$$ \bigcap_{n=1}^{\infty}(0,1/n)=\emptyset$$

Demostración. Asumamos por contradicción que 

$$x\in \bigcap_{n=1}^{\infty}(0,1/n)$$ 

Entonces para todo $n\in\mathbb{N}$: 
$$0< x <1/n$$
Pero como $x>0$, por la propiedad arquimediana sabemos que existe un $N\in \mathbb{N}$ tal que $(1/N) < x$. Pero esto significa que $x\notin (0, 1/N)$. Lo cual contradice que $x\in(0, 1/n)$ para todo $n$. Por lo tanto, no puede existir un elemento que pertenezca a la intersección.
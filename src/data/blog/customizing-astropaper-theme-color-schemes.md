---
author: MathDoggo
pubDatetime: 2022-09-25T15:20:35Z
modDatetime: 2026-01-09T15:00:15.170Z
title: Introducción a la Teoría de Juegos
featured: false
draft: false
tags:
  - Teoria de juegos
  - Matematicas Universitarias
  - Juego
  - Forma normal
description:
  Una muy pequeña introducción a la Teoría de Juegos.
---

La teoría de juegos es una colección de modelos matemáticos que nos ayudan a analizar situaciones donde interactúan múltiples agentes (jugadores) tomando decisiones. Estas decisiones están guiadas por las preferencias de cada jugador. El resultado depende de las decisiones de todos los agentes.

Este último detalle es precisamente lo que distingue a la teoría de juegos de los problemas clásicos de optimización, en los que suele existir un único agente, con ciertas restricciones, buscando maximizar o minimizar algún objetivo.

Para estudiar un juego, podemos considerar diferentes grados de cooperación entre los jugadores. Dos casos extremos son los juegos cooperativos, donde los jugadores pueden formar alianzas, y los juegos no cooperativos, donde cada jugador actúa por su cuenta. En esta saga nos enfocaremos exclusivamente en los juegos no cooperativos.

En este primer post vamos a formalizar lo que significa un juego.

Un juego $G$ es una terna

$$G=(N, (A^{i}), (u^{i})) \text{ con } i\in N$$

Donde:

- $N$ es el conjunto de jugadores,
- $A^{i}$ es el conjunto de estrategias para el jugador $i$
- $u^{i}:\prod_{i\in N}A^{i}\rightarrow \mathbb{R}$ es la función de utilidad para el jugador $i$

Es importante aclarar que en los juegos que vamos a estudiar las funciones de utilidad serán ordinales, es decir, solo sirven para distinguir el orden de las preferencias de cada jugador.

Por ejemplo, si yo soy un jugador y prefiero la estrategia $A$ sobre la estrategia $B$, basta con que $u(A)>u(B)$ no importa la cantidad por la que $u(A)$ sea mayor que $u(B)$.

Por último, cuando todos los jugadores eligen una estrategia podemos formar un conjunto con todas esas estrategias que generalmente se llama perfil de estrategias.

Ahora, matemáticamente el espacio de perfiles de estrategias se define como: 

$$Y = \prod_{i\in N} A^{i}$$ 

Cada $y\in Y$ es un perfil de estrategias.
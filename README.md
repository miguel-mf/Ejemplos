# Ejemplos

Algunos ejemplos de proyectos y cosas en las que he trabajado durante los últimos años.

## Trabajo en el Centro Sismológico Nacional: Fase W

Fuente: [Trabajo publicado](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/89/6/2237/548068/W-Phase-Real-Time-Implementation-and-Network?redirectedFrom=fulltext)

Un ejemplo de regresión multiparamétrica de datos. En este trabajo se buscaba encontrar parámetros físicos de un modelo de terremoto (epicentro, profundidad, magnitud, etc.) utilizando series de tiempo de datos sismológicos.

<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/FaseW.png" width="800">


Para esto se utilizó un modelo con regularización de tipo Ridge o Tikhonov de segundo orden en donde el parámetro de suavidad se determinó utilizando el método del codo o curva L con un set de datos preliminares. Este modelo nos permite pasar desde series de tiempo a un modelo físico de terremoto y así poder estimar de buena manera 

El resultado fue desplegar un software capaz de encontrar soluciones robustas para terremotos en tiempo real.




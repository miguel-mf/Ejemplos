# Ejemplos

Algunos ejemplos de proyectos y cosas en las que he trabajado durante los últimos años.

## Trabajo en el Centro Sismológico Nacional: Fase W

Fuente: [Trabajo publicado](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/89/6/2237/548068/W-Phase-Real-Time-Implementation-and-Network?redirectedFrom=fulltext)

Un ejemplo de regresión multiparamétrica de datos. En este trabajo se buscaba encontrar parámetros físicos de un modelo de terremoto (epicentro, profundidad, magnitud, etc.) utilizando series de tiempo de datos sismológicos.

<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/FaseW.png" width="800">


Para esto se utilizó un modelo con regularización de tipo Ridge o Tikhonov de segundo orden en donde el parámetro de suavidad se determinó utilizando el método del codo o curva L con un set de datos preliminares. Este modelo nos permite pasar desde series de tiempo a un modelo físico de terremoto y así poder estimar de buena manera 

El resultado fue desplegar un software capaz de encontrar soluciones robustas para terremotos en tiempo real.

## Trabajo en el Centro Sismológico Nacional: Alerta Temprana
Fuente: [Trabajo publicado](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/93/6/3337/616141)

Este fue un gran proyecto donde pusimos en marcha un software capaz de identificar rápidamente un terremoto mientras ocurre, de manera que seamos capaces de alertar a personas antes de que ellas perciban el sismo.

Este trabajo se separa en varias partes en particular en las que trabajé principalmente fueron diseño del software y creación de la aplicación móvil.

Parte del procesamiento es identificar en la señal si lo que vemos es un terremoto u otro tipo de señal, se utilizan métricas sobre la forma de la señal de manera de que un sistema de clasificación nos pueda indicar si es un sismo o no de manera rápida.

<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/Signals.gif" height="350"> 

Este sistema de clasificación fue entrenado utilizando la base de datos de terremotos identificados con anterioridad en el Centro Sismológico Nacional ~10.000 sismos por año registrado en ~100 estaciones y en 3 componentes, además probando señales sin sismos, ruidosas o con otro tipo de fenómenos.

<p float="left">
<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/SismosYear.jpg" width="420"> 
<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/SismosMag.jpg" width="420"> 
</p>

De esta manera podemos identificar sismos desde magnitud 2.0 en adelante de manera totalmente automática.

Por otra parte, una vez implementado el sistema se creo un prototipo de aplicación móvil para crear alertas más personalizadas. Esta aplicación fue desarrollada para Android/iOS con React Native.

<p float="left">
<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/Foto1.jpg" height="600"> 
<img src="https://github.com/miguel-mf/Ejemplos/blob/main/images/Foto2.jpg" height="600">
</p>

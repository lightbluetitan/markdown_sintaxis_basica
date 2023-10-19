---
title: "Sintaxis Básica Markdown"
subtitle: "Markdown - RMarkdown"
author: "Renzo Cáceres Rossi"
date: "2023/10/18"
output:
  html_document:
    code_download: TRUE
    toc: TRUE
    toc_float: TRUE
---

<!-- Crear documentos reproducibles con Markdown -->


## Sintaxis Markdown

**Markdown** es un lenguaje de marcado ligero (***Lightweight Markup Language***), siendo **RMarkdown**[^pie_pagina_01] uno de sus dialectos, uno de sus sabores (***Markdown Flavours***).

## Herramientas - Plataformas

- Lenguaje de programación R
- Python
- RStudio
- RPubs
- Netlifly
- GitHub Pages

## Encabezados - Títulos

```
# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
=========

Título 2
---------

```

## Separaciones - Líneas Horizontales

---

---

***

***


## Citas - Añadir citas a nuestro documento Markdown

> "La gente que está lo suficientemente loca para pensar que que pueden cambiar el mundo es la gente que lo consigue"
>
> **Steve Jobs**

## Formateo de texto - Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~

<u>Texto subrayado</u> <!-- HTML tags -->

## Listas

### Lista Viñetas - Lista Anidada

- Lista 1
- Lista 2
- Lista 3
- Lista 4
- Lista 5
  - Lista 5.1
  - Lista 5.2
  - Lista 5.3
- Lista 6
- Lista 7
- Lista 8

### Lista Numerada

1. Lista 1
2. Lista 2
3. Lista 3
4. Lista 4
5. Lista 5
6. Lista 6
7. Lista 7

### Lista ordenada alfabéticamente

a. Lista A
b. Lista B
c. Lista C
d. Lista D
e. Lista E
f. Lista F

### Lista Tareas

- [ ] Tarea A
- [ ] Tarea B
- [ ] Tarea C
- [ ] Tarea D
- [ ] Tarea E
- [ ] Tarea F

### Lista Casos - Ejemplos

- Lista 1
- Lista 2
- Lista 3
* Lista 4
* Lista 5
* Lista 6
+ Lista 7
+ Lista 8
+ Lista 9


## Enlaces - Añadir links a nuestro documento Markdown

<https://www.youtube.com/>

[YouTube](https://www.youtube.com/ "Ingresar YouTube")


[Renzo's YouTube Channel](https://www.youtube.com/c/RenzoCaceresRossi){target="_blank"}


## Imágenes - Añadir imágenes a nuestro documento Markdown

<!-- Añadir imágenes locales y online -->

<center>


![](diagrama_barras_amano.jpg){width=400 height=300}


![](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png){width=400 height=300}

</center>

## Tablas - Añadir tablas a nuestro documento Markdown


|TABLA A|TABLA B|TABLA C|
|:-----:|:-----:|:-----:|
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |

## Mapas - Añadir mapas (Google Maps) a nuestro documento Markdown

<center>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3901.973642551078!2d-77.03352652570888!3d-12.045334441872566!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8b5c8c412ef%3A0x70ab6fed9a118eb8!2sPalacio%20Municipal%20de%20Lima!5e0!3m2!1ses-419!2spe!4v1697692034898!5m2!1ses-419!2spe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" data-external=1></iframe>

</center>

<br>
<br>

## Vídeos - Añadir vídeos (YouTube) a nuestro documento Markdown

<center>

<iframe width="560" height="315" src="https://www.youtube.com/embed/C_UUnkTaV-Y?si=2QrcLQ4NHt0g5qe0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen data-external=1></iframe>


</center>

## Código - Añadir código de distintos lenguajes de programación (R-Python-SQL)

      summary(mtcars)
      
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.


~~~
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)
~~~

```R
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)
```

```Python
import matplotlib.pyplot as plt

eje_x=[4,6,8]

eje_y=[11,7,14]

colores =['orange','blue','purple']

plt.bar(eje_x,eje_y,colores,color=colores)

plt.xlabel('Cilindros')

plt.ylabel('Frecuencias')

plt.show()
```

```SQL
USE Northwind;

SELECT * FROM Products;
```

## Anular sintaxis Markdown


\**Esto debería ser texto formateado como Negrita**


\*Esto debería ser texto formateado como Cursiva*


\# Esto debería ser un título tipo 1


[^pie_pagina_01]: **RMarkdown es un paquete (package) del lenguaje de programación R que nos permite crear documentos reproducibles en distintos formatos tales como HTML,PDF o Microsoft Word**



<div class="tocify-extend-page" data-unique="tocify-extend-page" style="height: 0;"></div>


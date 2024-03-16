---
layout: post
title:  "Ecuación de segundo grado I"
date:   2024-01-10
excerpt: "Primera parte del curso de la ecuación de segundo grado en donde verás su dfinición, clasificación y métodos de resolución"
tag:
- Articulo
- Matematicas
- Blog
comments: false
---

Una ecuación es de **segundo grado** o **cuadrática** si el exponente de la incógnita es 2 (en otras palabras, \\( x^2 \\)).

## Forma estándar

La forma estándar de una ecuación cuadrática es la siguiente:

$$
\begin{align*}
ax^2 + bx + c &= 0
\end{align*}
$$

Donde:
* **a**, **b** y **c** son valores conocidos (también llamados coeficientes)
* **a** no puede ser igual a **0** (\\( a \neq 0 \\))
* **x** es la incógnita (el valor que estamos buscando)

### Ejemplos:

| Ecuación | Detalle | ¿Es de segundo grado? |
|:---:|:---:|:---:|
| \\( 2x^2 + 5x + 3 = 0 \\) | Los coeficientes **a**, **b** y **c** son distintos de 0 | Si |
| \\( -x^2 + x + 1 = 0 \\) | Los coeficientes **a**, **b** y **c** son distintos de 0 | Si |
| \\( 2x^2 - 72 = 0 \\) | El coeficiente **b** es igual a 0 | Si |
| \\( x^2 - 3x = 0 \\) | El coeficiente **c** es igual a 0 | Si |
| \\( x^2 = 0 \\) | Los coeficientes **b** y **c** son iguales a 0 | Si | 
| \\( 5x - 3 = 0 \\) | Ecuación lineal o de primer grado | No |
{: rules="groups"}

## Clasificación

Una ecuación cuadrática se puede clasificar en dos grupos:

### 1. Completa

Los coeficientes **a**, **b** y **c** son distintos de **0**, es decir, la ecuación tiene la forma:

$$
\begin{align*}
ax^2 + bx + c &= 0
\end{align*}
$$

### 2. Incompleta

Al menos uno de los coeficientes **b** y **c** es igual a **0**. En este grupo, encontraremos dos sub-grupos:

**2.1. Pura:** El coeficiente **b** es igual a **0**, es decir, la ecuación tiene la forma:

$$
\begin{align*}
ax^2 + c &= 0
\end{align*}
$$

**2.2. Binomial o Mixta:** El coeficiente **c** es igual a **0**, es decir, la ecuación tiene la forma:

$$
\begin{align*}
ax^2 + bx &= 0
\end{align*}
$$

## Resolución

Lo primero que debemos tener en cuenta es que en una ecuación cuadrática tendremos **2 soluciones**, las cuales pueden ser **distintas** o **iguales**. A estas soluciones también se les conoce como **raíces** o **ceros** de la ecuación.

### Resolución de ecuaciones incompletas

Hola amigos.

[MathJax](http://www.mathjax.org/) is a simple way of including Tex/LaTex/MathML based mathematics in HTML webpages. To get up and running you need to include the MathJax script in the header of your github pages page, and then write some maths. For LaTex, there are two delimiters you need to know about, one for block or displayed mathematics `\[ ... \]`, and the other for inline mathematics `\( ... \)`.

## Usage

To enable MathJax support be sure Kramdown is your Markdown flavor of choice and MathJax is set to true in your `_config.yml` file.

~~~
markdown: kramdown
mathjax: true
~~~

~~~
Here is an example MathJax inline rendering \\( 1/x^{2} \\), and here is a block rendering: 
\\[ \frac{1}{n^{2}} \\]
~~~

Here is an example MathJax inline rendering \\( 1/x^{2} \\), and here is a block rendering: 
\\[ \frac{1}{n^{2}} \\]

The only thing to look out for is the escaping of the backslash when using markdown, so the delimiters become `\\[ ... \\]` and `\\( ... \\)` for inline and block maths respectively.
    

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

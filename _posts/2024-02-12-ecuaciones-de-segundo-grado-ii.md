---
layout: post
title:  "Ecuaciones de Segundo Grado II"
date:   2024-02-12
excerpt: "Segunda parte del curso de Ecuaciones de Segundo Grado en donde verás la fórmula general de resolución, el discriminante y los tipos de soluciones."
tag:
- Articulo
- Matematicas
- Blog
comments: false
---

En esta segunda parte del curso de ecuaciones de segundo grado (si no has visto el capítulo anterior, te recomiendo hacer clic [aquí](https://elerizoinformatico.github.io/ecuaciones-de-segundo-grado-i/)) verás la fórmula general de resolución, el discriminante y los tipos de soluciones.

## Fórmula general

Las ecuaciones de segundo grado (cualquiera sea su tipo) podemos resolverlas mediante la fórmula general:

$$
\begin{align*}
x &= \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\end{align*}
$$

En donde el símbolo \\(\pm\\) nos indica que tendremos **dos** soluciones o raíces.

### Demostración de la fórmula general

Sea \\(ax^2 + bx + c = 0\\) nuestra ecuación de segundo grado o cuadrática (cualquiera sea su tipo) procederemos a **"despejar"** la incógnita \\(x\\):

$$
\begin{align*}
ax^2 + bx + c &= 0
\end{align*}
$$

Amplificamos por \\(4a\\):

$$
\begin{align*}
4a^2x^2 + 4abx + 4ac &= 0
\end{align*}
$$

Sumamos \\(b^2\\) en cada miembro de la igualdad:

$$
\begin{align*}
4a^2x^2 + 4abx + 4ac + b^2 &= b^2
\end{align*}
$$

Agrupamos términos de tal forma de obtener un **trinomio cuadrado perfecto**:

$$
\begin{align*}
4a^2x^2 + 4abx + b^2 &= b^2 - 4ac
\end{align*}
$$

Si \\((2ax + b)^2 = 4a^2x^2 + 4abx + b^2\\), entonces:

$$
\begin{align*}
(2ax + b)^2 &= b^2 - 4ac
\end{align*}
$$

Aplicamos raíz cuadrada en cada lado:

$$
\begin{align*}
\sqrt{(2ax + b)^2} &= \pm \sqrt{b^2 - 4ac}\\
2ax + b &= \pm \sqrt{b^2 - 4ac}
\end{align*}
$$

Por último, despejamos \\(x\\):

$$
\begin{align*}
x &= \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\end{align*}
$$

### Ejemplos

#### 1. \\(6x^2 - 5x + 1 = 0\\)

Como la ecuación está en su forma estándar (\\(ax^2 + bx + c = 0\\)), debemos identificar los valores de los coeficientes **a**, **b** y **c**:

\\(a = 6\\), \\(b = -5\\) y \\(c = 1\\)

Luego, reemplazamos los valores en la fórmula general y resolvemos:

$$
\begin{align*}
x &= \frac{-(-5) \pm \sqrt{(-5)^2 - 4\cdot(6)\cdot(1)}}{2\cdot(6)}\\
x &= \frac{5 \pm \sqrt{25 - 24}}{12}\\
x &= \frac{5 \pm \sqrt{1}}{12}\\
x &= \frac{5 \pm 1}{12}
\end{align*}
$$

Finalmente, las soluciones o raíces de la ecuación son:

$$
\begin{align*}
x_1 &= \frac{5 + 1}{12}\\
x_1 &= \frac{6}{12}\\
x_1 &= \frac{1}{2}
\end{align*}
$$

$$
\begin{align*}
x_2 &= \frac{5 - 1}{12}\\
x_2 &= \frac{4}{12}\\
x_2 &= \frac{1}{3}
\end{align*}
$$

#### 2. \\(8x + 5 = 36x^2\\)

En este caso, debemos ordenar la ecuación antes de identificar los coeficientes ya que no está en su forma estándar:

$$
\begin{align*}
8x + 5 &= 36x^2\\
36x^2 - 8x - 5 &= 0
\end{align*}
$$

**Importante:** Cuando resolvemos ecuaciones cuadráticas mediante la fórmula general, es recomendable que el valor del coeficiente **a** sea positivo para evitar errores en los cálculos.

Reemplazamos los valores en la fórmula general:

$$
\begin{align*}
x &= \frac{-(-8) \pm \sqrt{(-8)^2 - 4\cdot(36)\cdot(-5)}}{2\cdot(36)}\\
x &= \frac{8 \pm \sqrt{64 + 720}}{72}\\
x &= \frac{8 \pm \sqrt{784}}{72}\\
x &= \frac{8 \pm 28}{72}
\end{align*}
$$

Por lo tanto, las raíces de la ecuación son:

$$
\begin{align*}
x_1 &= \frac{8 + 28}{72}\\
x_1 &= \frac{36}{72}\\
x_1 &= \frac{1}{2}
\end{align*}
$$

$$
\begin{align*}
x_2 &= \frac{8 - 28}{72}\\
x_2 &= \frac{-20}{72}\\
x_2 &= - \frac{5}{18}
\end{align*}
$$

#### 3. \\((5x - 4)^2 - (3x + 5)(2x - 1) = 20x(x - 2) + 27\\)

Al igual que con el ejemplo anterior, la ecuación no se encuentra en su forma estándar y por lo mismo debemos ordenarla:

$$
\begin{align*}
(5x - 4)^2 - (3x + 5)(2x - 1) &= 20x(x - 2) + 27\\
(25x^2 - 40x + 16) - (6x^2 - 3x + 10x - 5) &= 20x^2 - 40x + 27\\
25x^2 - 40x + 16 - 6x^2 + 3x - 10x + 5 &= 20x^2 - 40x + 27\\
x^2 + 7x + 6 &= 0
\end{align*}
$$

Luego, reemplazamos los valores en la fórmula general:

$$
\begin{align*}
x &= \frac{-(7) \pm \sqrt{(7)^2 - 4\cdot(1)\cdot(6)}}{2\cdot(1)}\\
x &= \frac{-7 \pm \sqrt{49 - 24}}{2}\\
x &= \frac{-7 \pm \sqrt{25}}{2}\\
x &= \frac{-7 \pm 5}{2}
\end{align*}
$$

Por último, obtenemos sus raíces:

$$
\begin{align*}
x_1 &= \frac{-7 + 5}{2}\\
x_1 &= \frac{-2}{2}\\
x_1 &= -1
\end{align*}
$$

$$
\begin{align*}
x_2 &= \frac{-7 - 5}{2}\\
x_2 &= \frac{-12}{2}\\
x_2 &= -6
\end{align*}
$$

## Discriminante y tipos de soluciones

El **discriminante** (\\(\Delta\\)) corresponde al valor que se encuentra dentro de la raíz en la fórmula general de la ecuación cuadrática, es decir:

$$
\begin{align*}
\Delta &= b^2 - 4ac
\end{align*}
$$

A partir de este dato podemos conocer el tipo o naturaleza de sus raíces:

Hola amigos.

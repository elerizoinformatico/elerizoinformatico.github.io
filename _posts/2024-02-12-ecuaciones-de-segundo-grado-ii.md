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

A partir de este dato podemos conocer el tipo o **naturaleza** de sus raíces:

* Si \\(\Delta > 0\\), la ecuación tendrá dos soluciones **reales y distintas**, es decir, \\(x_1 \neq x_2\\).
* Si \\(\Delta = 0\\), la ecuación tendrá dos soluciones **reales e iguales**, es decir, \\(x_1 = x_2\\).
* Si \\(\Delta < 0\\), la ecuación **no tendrá solución en los reales**, es decir, \\(x_1\\) y \\(x_2\\) serán dos números **complejos conjugados**.

### Ejemplos

#### 1. \\(3x^2 - 5x + 1 = 0\\)

$$
\begin{align*}
\Delta &= (-5)^2 - 4\cdot(3)\cdot(1)\\
\Delta &= 25 - 12\\
\Delta &= 13
\end{align*}
$$

Ya que \\(\Delta = 13 > 0\\), podemos decir entonces que la ecuación tiene dos soluciones reales y distintas, las cuales estarán dadas por la fórmula general:

$$
\begin{align*}
x &= \frac{-b \pm \sqrt{\Delta}}{2a}
\end{align*}
$$

Es decir, los valores para \\(x_1\\) y \\(x_2\\) son:

$$
\begin{align*}
x_1 &= \frac{5 + \sqrt{13}}{6}
\end{align*}
$$

$$
\begin{align*}
x_2 &= \frac{5 - \sqrt{13}}{6}
\end{align*}
$$

#### 2. \\(x^2 - 4x + 4 = 0\\)

$$
\begin{align*}
\Delta &= (-4)^2 - 4\cdot(1)\cdot(4)\\
\Delta &= 16 - 16\\
\Delta &= 0
\end{align*}
$$

Como \\(\Delta = 0\\), la ecuación tendrá dos soluciones reales e iguales:

$$
\begin{align*}
x &= \frac{-b}{2a}\\
x &= \frac{4}{2}\\
x &= 2
\end{align*}
$$

#### 3. \\(x^2 + x + 1 = 0\\)

$$
\begin{align*}
\Delta &= (1)^2 - 4\cdot(1)\cdot(1)\\
\Delta &= 1 - 4\\
\Delta &= -3
\end{align*}
$$

En este caso,  \\(\Delta = -3 < 0\\) por lo que las soluciones de esta ecuación no están en los reales, es decir, serán dos números complejos conjugados:

$$
\begin{align*}
x_1 &= \frac{-1 + \sqrt{-3}}{2}
\end{align*}
$$

$$
\begin{align*}
x_2 &= \frac{-1 - \sqrt{-3}}{2}
\end{align*}
$$

## Ecuaciones cuadráticas a partir de sus soluciones

Si conocemos las raíces de una ecuación de segundo grado, podemos escribirla en su forma estándar como:

$$
\begin{align*}
x^2 - (x_1 + x_2)x + (x_1 \cdot x_2) &= 0
\end{align*}
$$

En donde sabemos que:

$$
\begin{align*}
x_1 + x_2 &= - \frac{b}{a}
\end{align*}
$$

$$
\begin{align*}
x_1 \cdot x_2 &= \frac{c}{a}
\end{align*}
$$

### Ejemplos

#### 1. \\(x_1 = 2\\) y \\(x_2 = 5\\)

$$
\begin{align*}
x^2 - (2 + 5)x + (2 \cdot 5) &= 0\\
x^2 - 7x + 10 &= 0
\end{align*}
$$

#### 2. \\(x_1 = -1\\) y \\(x_2 = 1/2\\)

$$
\begin{align*}
x^2 - (-1 + \frac{1}{2})x + (-1 \cdot \frac{1}{2}) &= 0\\
x^2 - (-\frac{1}{2})x + (-\frac{1}{2}) &= 0\\
x^2 + \frac{1}{2}x - \frac{1}{2} &= 0\\
2x^2 + x - 1 &= 0
\end{align*}
$$

#### 3. \\(x_1 = \sqrt{2}\\) y \\(x_2 = \sqrt{3}\\)

$$
\begin{align*}
x^2 - (\sqrt{2} + \sqrt{3})x + (\sqrt{2} \cdot \sqrt{3}) &= 0\\
x^2 - (\sqrt{2} + \sqrt{3})x + \sqrt{6} &= 0
\end{align*}
$$

## Ejercicios aplicados

1. \\(x^2 - 14x + 45 = 0\\)
2. \\(2x^2 - x - 1 = 0\\)
3. \\(6x^2 + 5x + 1 = 0\\)
4. \\(4x^2 - 9 = 0\\)
5. \\(2x^2 - 3x = 0\\)
6. \\(2x^2 + 5x + 2 = 0\\)
7. \\(x^2 + 1 = 0\\)
8. \\(x^2 + x + 1 = 0\\)
9. \\(x^2 - 2x + 2 = 0\\)
10. \\(1 - 3x(1 - x) = 0\\)
11. \\(x(x - 5) = 6\\)
12. \\(5x^2 + 3 = x^2 - 7x\\)
13. Para la ecuación \\(x^2 - 3x + k - 1 = 0\\), determina el valor de \\(k\\) tal que una de sus raíces sea igual a \\(0\\).
14. Para la ecuación \\(x^2 - kx + 36 = 0\\), determina el valor de \\(k\\) tal que sus raíces sean iguales.
15. Hallar el valor de dos números cuya suma sea \\(5\\) y su producto \\(-84\\).
16. Determinar la edad de Pedro sabiendo que dentro de 11 años tendrá la mitad del cuadrado de la edad que tenía hace 13 años.
17. Los \\(3\\) lados de un triángulo rectángulo son proporcionales a los números \\(3\\), \\(4\\) y \\(5\\). Calcula la longitud de cada lado sabiendo que tiene un área de \\(24m^2\\).
18. Un jardín rectangular de \\(50m\\) de largo por \\(34m\\) de ancho está rodeado por un camino de arena de ancho uniforme. Calcula la anchura de dicho camino si se sabe que tiene un área de \\(540m^2\\).
19. Calcula las dimensiones de un rectángulo cuya diagonal mide \\(75m\\) sabiendo que es semejante a otro rectángulo de \\(36m\\) por \\(48m\\).
20. Calcula dos números naturales cuya diferencia sea \\(2\\) y la suma de sus cuadrados \\(580\\).

Si tienes alguna duda con los contenidos vistos en este apartado o con los ejercicios aplicados, no dudes en escribirme en la caja de comentarios.

---

<script src="https://utteranc.es/client.js"
        repo="elerizoinformatico/elerizoinformatico.github.io"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>

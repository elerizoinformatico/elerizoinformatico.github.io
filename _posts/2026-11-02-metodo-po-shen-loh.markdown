---
layout: post
title:  "El método de Po-Shen Loh para ecuaciones cuadráticas"
date:   2026-11-02 22:21:47
---

En 2019, el matemático **Po-Shen Loh** (Carnegie Mellon University) popularizó una forma de resolver ecuaciones cuadráticas sin memorizar la fórmula general ni adivinar factorizaciones. Las ideas de fondo son antiguas (aparecen en escritos matemáticos babilónicos y en las relaciones de Vieta), pero Loh las organizó como un procedimiento directo e intuitivo.

La idea central es: **dos números cuya suma y producto conocemos son simétricos respecto de su promedio**.

### **El fundamento: las relaciones de Vieta**

Si una ecuación cuadrática **mónica** (coeficiente principal igual a 1):

$$
x^2 + bx + c = 0
$$

Tiene raíces $$r_1$$ y $$r_2$$, entonces puede escribirse como:

$$
(x - r_1)(x - r_2) = x^2 - (r_1 + r_2)\,x + r_1 r_2 = 0
$$

Comparando coeficientes se obtiene:

$$
r_1 + r_2 = -b \qquad\qquad r_1 \cdot r_2 = c
$$

Así, resolver la ecuación equivale a encontrar **dos números cuya suma es $$-b$$ y cuyo producto es $$c$$**.

### **La idea clave: simetría respecto del promedio**

Si dos números suman $$-b$$, su promedio es $$-\dfrac{b}{2}$$. Entonces uno está a cierta distancia $$u$$ por encima del promedio y el otro a la misma distancia por debajo:

$$
r_1 = -\frac{b}{2} + u \qquad\qquad r_2 = -\frac{b}{2} - u
$$

La suma se cumple automáticamente, cualquiera sea $$u$$:

$$
r_1 + r_2 = \left(-\frac{b}{2} + u\right) + \left(-\frac{b}{2} - u\right) = -b
$$

Solo falta imponer la condición del producto. Usando la diferencia de cuadrados $$(m+u)(m-u) = m^2 - u^2$$:

$$
\left(-\frac{b}{2} + u\right)\left(-\frac{b}{2} - u\right) = \frac{b^2}{4} - u^2 = c
$$

Despejando:

$$
u^2 = \frac{b^2}{4} - c
$$

Por lo tanto, las raíces son:

$$
\boxed{\,x = -\frac{b}{2} \pm \sqrt{\frac{b^2}{4} - c}\,}
$$

### **El procedimiento paso a paso**

1. **Normaliza:** si la ecuación es $$ax^2 + bx + c = 0$$ con $$a \neq 1$$, divide todo por $$a$$ para dejarla mónica.
2. **Identifica suma y producto:** las raíces suman $$-b$$ y multiplican $$c$$ (con los coeficientes ya normalizados).
3. **Calcula el promedio:** $$m = -\dfrac{b}{2}$$.
4. **Escribe las raíces como** $$m + u$$ y $$m - u$$.
5. **Plantea el producto:** $$m^2 - u^2 = c$$.
6. **Despeja** $$u^2 = m^2 - c$$ y luego $$u$$.
7. **Escribe las raíces:** $$x = m \pm u$$.
8. **Verifica** (opcional pero recomendado) que la suma y el producto coincidan.

### **Clasificación de las raíces según $$u^2$$**

El valor de $$u^2$$ cumple el mismo papel que el discriminante:

<table style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th style="border: 1px solid black; background-color: #f2f2f2; text-align: center;">$$u^2$$</th>
      <th style="border: 1px solid black; background-color: #f2f2f2; text-align: center;">Tipo de raíces</th>
      <th style="border: 1px solid black; background-color: #f2f2f2; text-align: center;">Forma</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid black; text-align: center;">$$u^2 > 0$$</td>
      <td style="border: 1px solid black; text-align: center;">Reales, distintas y racionales</td>
      <td style="border: 1px solid black; text-align: center;">$$m \pm u$$</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">$$u^2 > 0$$</td>
      <td style="border: 1px solid black; text-align: center;">Reales, distintas e irracionales</td>
      <td style="border: 1px solid black; text-align: center;">$$m \pm \sqrt{u^2}$$</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">$$u^2 = 0$$</td>
      <td style="border: 1px solid black; text-align: center;">Real doble (repetida)</td>
      <td style="border: 1px solid black; text-align: center;">$$x = m$$</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">$$u^2 < 0$$</td>
      <td style="border: 1px solid black; text-align: center;">Complejas conjugadas</td>
      <td style="border: 1px solid black; text-align: center;">$$m \pm i\sqrt{\lvert u^2 \rvert}$$</td>
    </tr>
  </tbody>
</table>

**Relación con el discriminante** $$\Delta = b^2 - 4c$$ (caso mónico):

$$
u^2 = \frac{b^2}{4} - c = \frac{b^2 - 4c}{4} = \frac{\Delta}{4}
$$

Por eso el signo de $$u^2$$ coincide con el signo de $$\Delta$$.

### **Conexión con la fórmula general**

Para $$ax^2 + bx + c = 0$$, al dividir por $$a$$:

$$
x^2 + \frac{b}{a}\,x + \frac{c}{a} = 0
$$

Aplicando el método con $$m = -\dfrac{b}{2a}$$:

$$
u^2 = \frac{b^2}{4a^2} - \frac{c}{a} = \frac{b^2 - 4ac}{4a^2}
\quad\Longrightarrow\quad
u = \frac{\sqrt{b^2 - 4ac}}{2a}
$$

$$
x = -\frac{b}{2a} \pm \frac{\sqrt{b^2 - 4ac}}{2a} = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

Es decir, **el método de Po-Shen Loh reconstruye la fórmula general** a partir de una idea intuitiva, sin necesidad de memorizarla.

### **Ejemplos**

**<u>Ejemplo 1</u>: Raíz real doble**

$$
x^2 + 6x + 9 = 0
$$

- $$x_1 + x_2 = -6$$ y $$x_1 \cdot x_2 = 9$$.
- $$m = -3$$.
- Raíces: $$-3 \pm u$$.
- $$u^2 = (-3)^2 - 9 = 0 \;\Rightarrow\; u = 0$$.

$$
x_1 = x_2 = -3 \quad \text{(raíz doble)}
$$

**Verificación:** $$(-3) + (-3) = -6$$ y $$(-3)(-3) = 9$$.

**<u>Ejemplo 2</u>: Raíces reales racionales distintas**

$$
x^2 - 8x + 15 = 0
$$

- $x_1 + x_2 = 8$$ y $$x_1 \cdot x_2 = 15$$.
- $$m = 4$$.
- Raíces: $$4 \pm u$$.
- $$u^2 = 4^2 - 15 = 1 \;\Rightarrow\; u = 1$$.

$$
x_1 = 5, \qquad x_2 = 3
$$

**Verificación:** $$5 + 3 = 8$$ y $$5 \cdot 3 = 15$$.

**Ejemplo 3: Raíces reales irracionales**

$$
x^2 - 4x + 1 = 0
$$

- Suma: $$4$$. Producto: $$1$$.
- Promedio: $$m = 2$$. Raíces: $$2 \pm u$$.
- Producto: $$4 - u^2 = 1$$.
- $$u^2 = 3 \;\Rightarrow\; u = \sqrt{3}$$.

$$
x_1 = 2 + \sqrt{3}, \qquad x_2 = 2 - \sqrt{3}
$$

**Verificación:** suma $$= 4$$; producto $$= 2^2 - (\sqrt{3})^2 = 4 - 3 = 1$$.

PDTE.

<script src="https://giscus.app/client.js"
        data-repo="elerizoinformatico/elerizoinformatico.github.io"
        data-repo-id="R_kgDONQWa5A"
        data-category="Ideas"
        data-category-id="DIC_kwDONQWa5M4CqaFl"
        data-mapping="pathname"
        data-strict="0"
        data-reactions-enabled="1"
        data-emit-metadata="0"
        data-input-position="bottom"
        data-theme="light_high_contrast"
        data-lang="es"
        crossorigin="anonymous"
        async>
</script>

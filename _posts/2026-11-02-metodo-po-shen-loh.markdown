---
layout: post
title:  "El método de Po-Shen Loh para ecuaciones cuadráticas"
date:   2026-11-02 22:21:47
---

En 2019, el matemático **Po-Shen Loh** (Carnegie Mellon University) popularizó una forma de resolver ecuaciones cuadráticas sin memorizar la fórmula general ni adivinar factorizaciones. Las ideas de fondo son antiguas (aparecen en escritos matemáticos babilónicos y en las relaciones de Vieta), pero Loh las organizó como un procedimiento directo e intuitivo.

La idea central es: **dos números cuya suma y producto conocemos son simétricos respecto de su promedio.**

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

PDTE

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

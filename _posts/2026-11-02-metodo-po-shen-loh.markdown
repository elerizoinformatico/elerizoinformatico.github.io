---
layout: post
title:  "El método de Po-Shen Loh para ecuaciones cuadráticas"
date:   2026-11-02 22:21:47
---

En 2019, el matemático **Po-Shen Loh** (Carnegie Mellon University) popularizó una forma de resolver ecuaciones cuadráticas sin memorizar la fórmula general ni adivinar factorizaciones. Las ideas de fondo son antiguas (aparecen en matemáticos babilónicos y en las relaciones de Vieta), pero Loh las organizó como un procedimiento directo e intuitivo.

La idea central es: **dos números cuya suma y producto conocemos son simétricos respecto de su promedio.**

### El fundamento: las relaciones de Vieta

Si una ecuación cuadrática **mónica** (coeficiente principal igual a 1):

$$
x^2 + bx + c = 0
$$

Tiene raíces $r_1$ y $r_2$, entonces puede escribirse como:

$$
(x - r_1)(x - r_2) = x^2 - (r_1 + r_2)\,x + r_1 r_2 = 0 .
$$

Comparando coeficientes se obtiene:

$$
r_1 + r_2 = -b \qquad\qquad r_1 \cdot r_2 = c
$$

Así, resolver la ecuación equivale a encontrar **dos números cuya suma es $-b$ y cuyo producto es $c$.**

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

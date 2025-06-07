---
layout: post
title:  "Determinando si un número es primo con recursividad"
date:   2025-01-03 19:01:37
---

Ya sabemos que un **número primo** es cualquier número entero positivo mayor que 1 que sólo puede ser dividido por 1 y por si mismo.

En el mundo de la programación nos encontraremos con muchos códigos que nos permiten determinar si un número es primo o no mediante iteraciones (ciclos `for` o `while`). Sin embargo, en esta ocasión traemos a la mesa una solución mediante la **recursividad**:

{% highlight python %}
def es_primo(num, divisor=2):
    if num < 2:
        return False
    if divisor * divisor > num:
        return True
    if num % divisor == 0:
        return False
    return es_primo(num, divisor + 1)

# Solicitar número al usuario
try:
    numero = int(input("Ingresa un número entero: "))
    if es_primo(numero):
        print(f"{numero} es un número primo.")
    else:
        print(f"{numero} no es un número primo.")
except ValueError:
    print("Por favor, ingresa un número entero válido.")
{% endhighlight %}

## ¿Cómo funciona?

* La función `es_primo` usa un segundo parámetro `divisor` que comienza en 2.
* Si el número es menor que 2 no es primo.
* Si el cuadrado de `divisor` es mayor que el número, no se encontró ningún divisor y por lo tanto es primo.
* Si el número es divisible por `divisor`, no es primo.
* Si no, la función se llama a sí misma con `divisor + 1`.

Se ve interesante el código aunque analizaremos su complejidad (orden de crecimiento):

La función `es_primo` prueba todos los divisores desde 2 hasta $\sqrt{num}$, haciendo una llamada recursiva por cada intento. En el peor caso, se ejecuta hasta que `divisor * divisor > num`, es decir, prueba divisores hasta $divisor = \sqrt{num}$. Entonces, la complejidad es:

$$ Complejidad = O(\sqrt{n}) $$

## ¿Se puede mejorar?

Claro que si, podríamos considerar:

* Probar solo divisores impares después del 2.
* Usar pruebas de primalidad más avanzadas (como Miller-Rabin) si se requiere eficiencia en números grandes.

¿Tienes alguna otra idea para mejorar su eficiencia? ¡Déjalo en los comentarios!

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
---
layout: post
title:  "Método Bubble Sort y su complejidad"
date:   2025-02-13 19:39:43
---

El **Bubble Sort** o **Método de la Burbuja** es un algoritmo de ordenamiento basado en comparaciones sucesivas de elementos adyacentes en una lista o arreglo.

### **¿Cómo funciona?**

1. Compara el primer elemento con el segundo.
2. Si están en el orden incorrecto (por ejemplo, el primero es mayor que el segundo), los intercambia.
3. Repite esto con todos los pares adyacentes hasta el final del arreglo.
4. Eso cuenta como **una pasada**. Luego repite el proceso pero sin considerar el último elemento (porque ya está en su lugar).
5. Se repite este proceso hasta que ya no se hacen más intercambios, lo que significa que el arreglo está ordenado.

### **Implementación en Python**

El algoritmo a continuación genera un arreglo de `n` elementos (todos números enteros aleatorios entre `0` y `n-1`), ordena los elementos mediante Bubble Sort y mide el tiempo que tarda en ejecutar esta tarea. Su propósito es verificar los tiempos de ejecución a medida que aumentamos la cantidad de elementos para determinar de forma gráfica su complejidad u orden de crecimiento:

{% highlight python %}
import random
import time

def generar_array(tamano, minimo, maximo):
    return [random.randint(minimo, maximo) for _ in range(tamano)]

def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]

def tiempo_ordenamiento(func, arr):
    inicio = time.time()
    func(arr)
    fin = time.time()
    return fin - inicio

try:
    tamano = int(input("Ingrese tamaño del arreglo: "))
    minimo = 0
    maximo = tamano - 1

    if minimo > maximo:
        raise ValueError("El valor mínimo no puede ser mayor que el máximo.")
    
    arreglo = generar_array(tamano, minimo, maximo)
    #print(f"\nArreglo original:\n{arreglo}")

    duracion = tiempo_ordenamiento(bubble_sort, arreglo)

    #print(f"\nArreglo ordenado:\n{arreglo}")
    print(f"Tiempo de ejecución del ordenamiento para {tamano} elementos: {duracion:.6f} seg")

except ValueError as e:
    print(f"Error: {e}")
{% endhighlight %}

### **Resultados**

Para los tamaños ingresados se ejecutó el algoritmo 3 veces ya que el arreglo generado es aleatorio y por lo mismo, los tiempos de ejecución pueden variar. Los resultados (en segundos) se presentan a continuación:

<table style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th style="border: 1px solid black; background-color: #f2f2f2; text-align: center;">N° de elementos</th>
      <th style="border: 1px solid black; text-align: center;">Tiempo 1</th>
      <th style="border: 1px solid black; text-align: center;">Tiempo 2</th>
      <th style="border: 1px solid black; text-align: center;">Tiempo 3</th>
      <th style="border: 1px solid black; text-align: center;">Promedio</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid black; text-align: center;">1000</td>
      <td style="border: 1px solid black; text-align: center;">0.039926</td>
      <td style="border: 1px solid black; text-align: center;">0.028880</td>
      <td style="border: 1px solid black; text-align: center;">0.025517</td>
      <td style="border: 1px solid black; text-align: center;">0.031441</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">2000</td>
      <td style="border: 1px solid black; text-align: center;">0.115584</td>
      <td style="border: 1px solid black; text-align: center;">0.119061</td>
      <td style="border: 1px solid black; text-align: center;">0.124567</td>
      <td style="border: 1px solid black; text-align: center;">0.119737</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">3000</td>
      <td style="border: 1px solid black; text-align: center;">0.275539</td>
      <td style="border: 1px solid black; text-align: center;">0.272289</td>
      <td style="border: 1px solid black; text-align: center;">0.269378</td>
      <td style="border: 1px solid black; text-align: center;">0.272402</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">4000</td>
      <td style="border: 1px solid black; text-align: center;">0.496379</td>
      <td style="border: 1px solid black; text-align: center;">0.504710</td>
      <td style="border: 1px solid black; text-align: center;">0.491834</td>
      <td style="border: 1px solid black; text-align: center;">0.497641</td>
    </tr>
    <tr>
      <td style="border: 1px solid black; text-align: center;">5000</td>
      <td style="border: 1px solid black; text-align: center;">0.781531</td>
      <td style="border: 1px solid black; text-align: center;">0.781016</td>
      <td style="border: 1px solid black; text-align: center;">0.800987</td>
      <td style="border: 1px solid black; text-align: center;">0.787845</td>
    </tr>
  </tbody>
</table>

Si realizamos una gráfica, obtenemos una curva similar a la función cuadrática o parábola:

<img src="{{ site.baseurl }}/assets/img/grafica1.png">

### **Complejidad**

La eficiencia de un algoritmo  se mide por su **complejidad de tiempo** (cuánto tiempo toma) y su **complejidad de espacio** (cuánta memoria necesita). Para el Bubble Sort, la complejidad de tiempo es su principal desventaja:

#### **Complejidad de Tiempo**

* **Peor caso** $$O(n^{2})$$: Ocurre cuando la lista está en orden inverso. El algoritmo debe recorrer toda la lista $$n$$ veces y en cada pasada realiza hasta $$n$$ comparaciones. Esto genera un número de operaciones proporcional a $$n \cdot n$$, es decir, crecimiento cuadrático.
* **Caso promedio** $$O(n^{2})$$: Incluso con un orden aleatorio, el algoritmo sigue siendo ineficiente ya que el número de comparaciones e intercambios sigue siendo cuadrático en función del tamaño de la lista.
* **Mejor caso** $$O(n)$$: Sucede cuando la lista ya está ordenada. En este escenario, el algoritmo recorre la lista una sola vez y, al no detectar ningún intercambio, finaliza anticipadamente.

#### **Complejidad de Espacio**

Bubble Sort es un algoritmo **in-place** (en el lugar), lo que significa que no requiere estructuras de datos adicionales. Todos los intercambios se realizan directamente en el mismo arreglo original, utilizando solo una cantidad constante de memoria adicional.

Si te diste cuenta, Bubble Sort es bastante ineficiente para listas grandes y por lo mismo su uso en aplicaciones prácticas es bastante raro. Su principal utilidad es como herramienta pedagógica para introducir los conceptos básicos de los algoritmos de ordenamiento.

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

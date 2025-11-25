---
layout: post
title:  "Juego del Cachipún en Python"
date:   2025-11-21 18:01:14
---

En esta ocasión, vamos a programar el mítico juego del **"Cachipún"** o **"Piedra, Papel o Tijera"** con un sencillo código en Python.

Para implementar este juego, utilizaremos el método random para que genere automáticamente la **"jugada"** de la máquina:

{% highlight python %}
import random

while True:
    aleatorio = random.randrange(0, 3)
    eligePc = ""
    print("1. Piedra")
    print("2. Papel")
    print("3. Tijera")
    opcion = int(input("Elige tu opción: "))

    if opcion == 1:
        eligeUsuario = "Piedra"
    elif opcion == 2:
        eligeUsuario = "Papel"
    elif opcion == 3:
        eligeUsuario = "Tijera"
    print("Elejiste: ", eligeUsuario)

    if aleatorio == 0:
        eligePc = "Piedra"
    elif aleatorio == 1:
        eligePc = "Papel"
    elif aleatorio == 2:
        eligePc = "Tijera"
    print("La máquina eligió: ", eligePc)
    print("...")

    if eligePc == "Piedra" and eligeUsuario == "Papel":
        print("Ganaste, Papel envuelve Piedra")
    elif eligePc == "Papel" and eligeUsuario == "Tijera":
        print("Ganaste, Tijera corta Papel")
    elif eligePc == "Tijera" and eligeUsuario == "Piedra":
        print("Ganaste, Piedra machaca Tijera")
    elif eligePc == "Papel" and eligeUsuario == "Piedra":
        print("Perdiste, Papel envuelve Piedra")
    elif eligePc == "Tijera" and eligeUsuario == "Papel":
        print("Perdiste, Tijera corta Papel")
    elif eligePc == "Piedra" and eligeUsuario == "Tijera":
        print("Perdiste, Piedra machaca Tijera")
    elif eligePc == eligeUsuario:
        print("Empate")
    
    jugar_otra_vez = input("¿Quieres jugar de nuevo? (s/n): ")
    if jugar_otra_vez.lower() != "s":
        break
{% endhighlight %}

El código es muy sencillo, por una parte generamos un número aleatorio con `random` entre `0` y `3` que será la jugada de la máquina. Después, con un simple menú haremos nuestra elección y luego solo hay que contemplar todas las opciones con el condicional `if`.

Por otra parte, si queremos jugar varias veces, solo tendremos que introducir un bucle `while` en el juego con la típica pregunta **si o no** al final.

### Versión 2.0

Podemos "aprovechar" las características de Python para **mejorar** el código:

{% highlight python %}
import random

def obtener_ganador(jugador, maquina):
    # Reglas del juego
    reglas = {
        "piedra": "tijeras",
        "papel": "piedra",
        "tijeras": "papel"
    }

    if jugador == maquina:
        return "Empate"
    elif reglas[jugador] == maquina:
        return "Ganaste"
    else:
        return "Perdiste"

def jugar():
    opciones = ["piedra", "papel", "tijeras"]

    print("=== Piedra, Papel o Tijeras ===")
    jugador = input("Elige (piedra, papel o tijeras): ").lower()

    # Validar entrada
    while jugador not in opciones:
        jugador = input("Opción inválida. Elige (piedra, papel o tijeras): ").lower()

    maquina = random.choice(opciones)
    print(f"La máquina eligió: {maquina}")

    resultado = obtener_ganador(jugador, maquina)
    print(f"Resultado: {resultado}")

if __name__ == "__main__":
    jugar()
{% endhighlight %}

Principales características:
* Validación de entrada: evitamos que el usuario ingrese valores fuera de las opciones.
* Lógica limpia ya que utilizamos un diccionario de reglas.
* Función modularizada para reutilización de código o pruebas.
* Modo ejecutable con `if __name__ == "__main__":`

Ambos programas cumplen la misma función, pero su principal diferencia radica en que la **primera versión es menos ordenada y más repetitiva**, mientras que la **segunda versión es más limpia y fácil de testear o reutilizar**.

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
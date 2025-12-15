# Examen de Depuración en PyCharm

---

## **Instrucciones:**

1. Realiza un fork de este repositorio y clónalo.
1. Las respuestas a las preguntas realízalas en este Readme
2. Cada pregunta vale un punto

### Apartado 1

- Coloca un punto de interrupción **normal** en la línea donde se inicializa la lista de la serie: `serie = [0, 1]`.

![Captura desde 2025-12-15 13-59-31.png](../../Im%C3%A1genes/Capturas%20de%20pantalla/Captura%20desde%202025-12-15%2013-59-31.png)

- Inicia el modo *Debug*.

![Captura desde 2025-12-15 14-02-17.png](../../Im%C3%A1genes/Capturas%20de%20pantalla/Captura%20desde%202025-12-15%2014-02-17.png)

**Pregunta**

1. Si la función es llamada con `n=10`, ¿cuál es el valor de la variable `n` que se visualiza en la ventana de variables del debugger justo antes de que se ejecute la línea `serie = [0, 1]`?
   ![Captura desde 2025-12-15 14-22-43.png](../../Im%C3%A1genes/Capturas%20de%20pantalla/Captura%20desde%202025-12-15%2014-22-43.png)
---

### Apartado 2

-  Asegúrate de que la llamada a la función es `print(funcion_bucle(10))`.
-  Inicia el modo *Debug* y avanza hasta que la ejecución se detenga en la línea `siguiente_numero = calcular_siguiente(serie)`.
-  Utiliza la opción de depuración adecuada para **entrar dentro** de la función `calcular_siguiente`.

**Preguntas**

1. Justo cuando el debugger se detiene dentro de la función `calcular_siguiente` por **primera vez**, ¿cuál es el valor que tiene la variable local `aux` *después* de que se ejecute la línea `aux = serie[-1] + serie[-2]`?

[0,1]

**(Indica el valor numérico exacto de la variable `aux` en ese momento y el nombre de la herramienta de *debugging* que utilizaste para entrar en la función).**


2. Si estuvieras dentro de la función `calcular_siguiente` y quisieras salir rápidamente sin ejecutar el resto de las líneas, volviendo al punto de llamada en `funcion_bucle`, ¿qué función del debugger deberías usar?

step out

3. ¿Qué diferencia fundamental existe entre usar *Step Over* y *Step Into* en la línea `siguiente_numero = calcular_siguiente(serie)`?
step into entra en la funcion y la ejecuta, step over ejecuta la funcion sin entrar en ella
---

### Apartado 3

-  Cambia la llamada a la función para que el número de elementos sea mayor: `print(funcion_bucle(1000))`.
-  Establece un **Breakpoint Condicional** para que la ejecución se detenga solo cuando `siguiente_numero` sea **mayor que 20000**.

**Pregunta**

1. Cuando el *Breakpoint Condicional* se activa por **primera vez** (la primera vez que `siguiente_numero` es mayor que 20000), ¿qué longitud tiene `serie`?
24
---

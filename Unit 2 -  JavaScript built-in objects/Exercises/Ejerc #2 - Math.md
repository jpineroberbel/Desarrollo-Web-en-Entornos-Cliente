# 📝 Ejercicios con `Math` en JavaScript

## Nivel 1 – Básicos
1. **Número absoluto**  
   Escribe una función que reciba un número y devuelva su valor absoluto usando `Math.abs`.

2. **Redondeo simple**  
   Pide al usuario un número decimal y muestra:  
   - Su valor redondeado (`Math.round`)  
   - Su redondeo por exceso (`Math.ceil`)  
   - Su redondeo por defecto (`Math.floor`)

3. **Potencias y raíces**  
   - Calcula \( 5^3 \) con `Math.pow`.  
   - Calcula la raíz cuadrada de 81 con `Math.sqrt`.

4. **Valor máximo y mínimo**  
   Dado el array `[10, -5, 3, 99, 42]`, encuentra el número más grande y el más pequeño usando `Math.max` y `Math.min`.

---

## Nivel 2 – Aleatoriedad
5. **Número aleatorio entre 0 y 1**  
   Genera un número aleatorio con `Math.random` y muéstralo.

6. **Dado virtual (1–6)**  
   Usa `Math.random` y `Math.floor` para simular el lanzamiento de un dado que devuelva un número del 1 al 6.

7. **Número aleatorio en un rango**  
   Crea una función que reciba dos números (`min`, `max`) y devuelva un número entero aleatorio en ese rango.

---

## Nivel 3 – Trigonometría y logaritmos
8. **Seno y coseno**  
   Calcula el seno y coseno de 45° (recuerda que `Math.sin` y `Math.cos` trabajan en radianes, no en grados).

9. **Tangente y arco tangente**  
   - Calcula la tangente de 60°.  
   - Convierte un valor usando `Math.atan` a grados.

10. **Logaritmos**  
   - Calcula el logaritmo natural de 10 (`Math.log`).  

---

## Nivel 4 – Retos aplicados
11. **Juego: adivina el número**  
   Genera un número aleatorio entre 1 y 100 y pide al usuario adivinarlo. Indica si el número ingresado es mayor o menor hasta que acierte.

12. **Distancia entre dos puntos**  
   Dadas las coordenadas `(x1, y1)` y `(x2, y2)`, calcula la distancia usando la fórmula:  
   \[
   \sqrt{(x2 - x1)^2 + (y2 - y1)^2}
   \]

13. **Simulación de ruleta**  
   Simula una ruleta que tenga 36 números. Usa `Math.random` para elegir el número ganador.

14. **Generador de contraseñas simples**  
   Usa `Math.random` y un conjunto de caracteres para crear una contraseña aleatoria de 8 caracteres.

# Relación de Ejercicios Avanzados de Bucles en JavaScript

> **Indicaciones para el alumnado:**  
> En esta relación de ejercicios no se permite el uso de métodos auxiliares de orden superior de arrays (como `.map()`, `.filter()`, `.reduce()`, `.forEach()`) ni métodos directos de cadena como `.repeat()`.  
> **El objetivo principal es resolver la lógica del problema aplicando estructuras repetitivas nativas (`for`, `while`, `do...while`) y optimizando el número de iteraciones.**

---

### 1. Patrones dinámicos: El Rombo
Dado un número entero impar $n$ (por ejemplo, $n = 7$), dibuja en la consola un rombo perfecto de asteriscos.

* **Ejemplo de entrada:** `n = 5`
* **Salida esperada:**
  ```text
    *
   ***
  *****
   ***
    *
  ```
* **Pista:** Calcula en un bucle la cantidad de espacios y asteriscos que corresponden a cada fila $i$.

---

### 2. Ordenación manual (Algoritmo de Burbuja)
Dado un array de números desordenados, ordénalo de menor a mayor **sin utilizar** `Array.prototype.sort()`.

* **Ejemplo de entrada:** `[5, 2, 9, 1, 5, 6]`
* **Salida esperada:** `[1, 2, 5, 5, 6, 9]`
* **Pista:** Utiliza bucles `for` anidados para comparar elementos adyacentes e intercambiar sus posiciones (*swapping*) si están desordenados.

---

### 3. Criba de Eratóstenes (Primos eficientes)
Dado un número entero $N$, genera todos los números primos menores o iguales a $N$ aplicando el algoritmo histórico de la criba de Eratóstenes.

* **Ejemplo de entrada:** `N = 30`
* **Salida esperada:** `[2, 3, 5, 7, 11, 13, 17, 19, 23, 29]`
* **Pista:** Crea un array de booleanos de tamaño $N+1$ inicializado a `true`. Utiliza un bucle para ir marcando como `false` los múltiplos de cada primo encontrado.

---

### 4. Compresión de cadenas (Run-Length Encoding)
Crea una función que tome una cadena de caracteres repetidos y devuelva su versión comprimida. Si la cadena comprimida no resulta ser más corta que la original, debe devolver la cadena original.

* **Ejemplo de entrada:** `"aabcccccaaa"`
* **Salida esperada:** `"a2b1c5a3"`
* **Pista:** Recorre la cadena con un solo bucle manteniendo un contador de la letra actual y comparándola con el carácter en la posición `i + 1`.

---

### 5. Validación de Matriz Identidad
Escribe una función que reciba una matriz bidimensional (array de arrays) de $N \times N$ y determine mediante bucles si es una **Matriz Identidad** (1s en la diagonal principal y 0s en el resto).

* **Ejemplo de entrada:** 
  ```javascript
  [
    [1, 0, 0],
    [0, 1, 0],
    [0, 0, 1]
  ]
  ```
* **Salida esperada:** `true`
* **Pista:** Usa un bucle anidado (`i`, `j`) y aplica una salida temprana (`return false`) en cuanto encuentres un elemento que no cumpla la condición.

---

### 6. Recorrido de Matriz en Espiral (Caracol)
Dada una matriz bidimensional de $N \times M$, devuelve todos sus elementos recorriéndola en sentido de las agujas del reloj (de fuera hacia dentro).

* **Ejemplo de entrada:**
  ```javascript
  [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
  ]
  ```
* **Salida esperada:** `[1, 2, 3, 6, 9, 8, 7, 4, 5]`
* **Pista:** Define 4 variables límite (`filasInicio`, `filasFin`, `colsInicio`, `colsFin`) y actualízalas dentro de un bucle `while` a medida que recorres los bordes.

---

### 7. Conversión de Números Integreos a Romanos
Convertir un entero entre 1 y 3999 a su representación en números romanos usando exclusivamente bucles y una tabla de equivalencias.

* **Ejemplo de entrada:** `1984`
* **Salida esperada:** `"MCMLXXXIV"`
* **Pista:** Utiliza el enfoque del *algoritmo voraz*: en cada paso de un bucle `while`, resta el valor más grande posible del número original y concatena el símbolo romano correspondiente.

---

### 8. Detector de Palíndromos mediante Dos Punteros
Determina si una frase es un palíndromo (ignorando espacios, mayúsculas y tildes) utilizando **un solo bucle** y el patrón de dos punteros (*Two Pointers*).

* **Ejemplo de entrada:** `"Anilina"` o `"Dabale arroz a la zorra el abad"`
* **Salida esperada:** `true`
* **Pista:** Inicializa un puntero `inicio = 0` y otro `fin = cadena.length - 1`. En cada iteración del bucle, avanza el inicio y retrocede el fin comparando ambos caracteres.

---

### 9. Búsqueda Binaria Iterativa
Dado un array de números previamente **ordenado** de 1000 elementos y un número objetivo, implementa la búsqueda binaria mediante un bucle `while` para devolver el índice del valor en tiempo $\mathcal{O}(\log n)$.

* **Ejemplo de entrada:** `array = [2, 5, 8, 12, 16, 23, 38, 56, 72, 91]`, `target = 23`
* **Salida esperada:** `5` (índice donde se encuentra el 23)
* **Pista:** Mantén variables para el límite `izq` y `der`. En cada paso calcula el punto medio `mid` y descarta la mitad del array que no contenga el valor.

---

### 10. Juego de la Vida de Conway (1 Generación)
Dada una rejilla de $5 \times 5$ representada por una matriz de `0` (celda muerta) y `1` (celda viva), calcula el estado de la rejilla en la siguiente generación.

* **Reglas:**
  1. Celda viva con $< 2$ vecinas vivas: Muere (soledad).
  2. Celda viva con 2 o 3 vecinas vivas: Sobrevive.
  3. Celda viva con $> 3$ vecinas vivas: Muere (superpoblación).
  4. Celda muerta con exactamente 3 vecinas vivas: Nace (reproducción).
* **Pista:** Para cada posición `(i, j)`, utiliza un doble bucle de $-1$ a $+1$ para contar los vecinos vivos alrededor, asegurándote de no comprobar posiciones fuera de los límites de la matriz.
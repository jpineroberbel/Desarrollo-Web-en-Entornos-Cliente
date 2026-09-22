# Relación de Ejercicios: El Operador Ternario en JavaScript

> **Indicaciones para el alumnado:**
>
> El operador ternario (`condición ? expresión_si_verdadero : expresión_si_falso`) es una alternativa concisa a las estructuras `if...else`. Recuerda que el operador ternario **devuelve un valor** (es una expresión), por lo que es ideal para asignaciones directas, retornos de funciones e interpolación de cadenas.
>
> **Objetivo:** Resolver los siguientes retos manteniendo el código conciso, legible y aplicando buenas prácticas de sintaxis.

### 1. Par o Impar

Crea una función o expresión que determine si un número entero es par o impar.

* **Ejemplo de entrada:** `7`
* **Salida esperada:** `"Impar"`
* **Reto:** Resuélvelo en una sola línea utilizando el operador de módulo `%`.

---

### 2. Asignador de Descuentos (Ternario encadenado)

Calcula el porcentaje de descuento a aplicar según los puntos acumulados por un cliente:

* Más de 100 puntos $\rightarrow$ **20%**
* Entre 50 y 100 puntos $\rightarrow$ **10%**
* Menos de 50 puntos $\rightarrow$ **0%**

* **Ejemplo de entrada:** `puntos = 75`
* **Salida esperada:** `10`
* **Reto:** Aplica una estructura de ternarios anidados cuidando la legibilidad.

---

### 3. Validador de Acceso

Determina si un usuario cumple los requisitos para subir a una atracción de parque temático. La regla exige tener **al menos 18 años** O medir **más de 160 cm**.

* **Ejemplo de entrada:** `edad = 16`, `altura = 170`
* **Salida esperada:** `"Acceso permitido"`
* **Reto:** Combina operadores lógicos (`||`, `&&`) dentro de la condición evaluada.

---

### 4. Valor por Defecto con Fallback

Dada una variable `username` que puede contener una cadena de texto o los valores `null` / `undefined`, asigna el nombre de usuario o la cadena `"Invitado"` si no está definido.

* **Ejemplo de entrada:** `username = null`
* **Salida esperada:** `"Invitado"`


---

### 5. Conversor de Calificaciones

Dada una nota numérica entre 0 y 10, devuelve la calificación cualitativa equivalente:

* Nota $\ge 9 \rightarrow$ `"Sobresaliente"`
* Nota $\ge 7 \rightarrow$ `"Notable"`
* Nota $\ge 5 \rightarrow$ `"Aprobado"`
* Nota $< 5 \rightarrow$ `"Suspenso"`

* **Ejemplo de entrada:** `8.5`
* **Salida esperada:** `"Notable"`
* **Reto:** Formatea la secuencia de ternarios encadenados de forma vertical e intuitiva.

---

### 6. Calculadora de Gastos de Envío

Dado el valor total de una cesta de compra, calcula el importe final. Si la compra es superior a 50€, el envío es gratuito ($0€$); en caso contrario, se aplican $4.95€$ de gastos de envío.

* **Ejemplo de entrada:** `totalCompra = 35`
* **Salida esperada:** `39.95`
* **Reto:** Realiza la suma/operación aritmética directamente en el retorno del ternario.

---

### 7. Normalizador de Rangos (Clamp)

Dado un valor `val`, restringe su rango para que se mantenga entre $[0, 100]$. Si es menor que $0$, devuelve $0$; si es mayor que $100$, devuelve $100$; en cualquier otro caso, devuelve el propio valor.

* **Ejemplo de entrada:** `val = 145`
* **Salida esperada:** `100`
* **Reto:** Implementa la lógica de acotación (*clamp*) en una sola línea utilizando dos ternarios.

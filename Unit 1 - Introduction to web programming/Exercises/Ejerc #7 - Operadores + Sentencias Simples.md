# Relación de Ejercicios en JavaScript
**Objetivo:** Practicar operadores, expresiones, condicionales y bucles usando sentencias simples.

---

## Ejercicio 1: Suma de números
**Objetivo:** Practicar operadores aritméticos.  
**Enunciado:** Crea un programa que pida al usuario dos números y muestre la suma, resta, multiplicación y división de ambos.

```javascript
let num1 = Number(prompt("Ingrese el primer número"));
let num2 = Number(prompt("Ingrese el segundo número"));

// Tu código aquí para mostrar suma, resta, multiplicación y división
```

---

## Ejercicio 2: Determinar par o impar
**Objetivo:** Practicar operadores de módulo (%) y condicionales.  
**Enunciado:** Pide al usuario un número e indica si es **par** o **impar**.

```javascript
let numero = Number(prompt("Ingrese un número"));
// Usa un condicional para determinar si es par o impar
```

---

## Ejercicio 3: Mayor de tres números
**Objetivo:** Practicar operadores de comparación y condicionales.  
**Enunciado:** Pide al usuario tres números e indica cuál es el mayor.

```javascript
let a = Number(prompt("Número 1"));
let b = Number(prompt("Número 2"));
let c = Number(prompt("Número 3"));
// Escribe un condicional para encontrar el mayor
```

---

## Ejercicio 4: Tabla de multiplicar
**Objetivo:** Practicar bucles y operadores.  
**Enunciado:** Pide un número y muestra su tabla de multiplicar del 1 al 10.

```javascript
let num = Number(prompt("Ingrese un número"));
// Usa un bucle for para mostrar la tabla de multiplicar
```

---

## Ejercicio 5: Suma de números del 1 al N
**Objetivo:** Practicar bucles y acumuladores.  
**Enunciado:** Pide un número N e imprime la suma de todos los números del 1 hasta N.

```javascript
let N = Number(prompt("Ingrese un número"));
// Usa un bucle for y una variable acumuladora para sumar
```

---

## Ejercicio 6: Contador de números positivos y negativos
**Objetivo:** Practicar condicionales dentro de bucles.  
**Enunciado:** Pide 5 números y cuenta cuántos son positivos y cuántos negativos.

```javascript
let positivos = 0;
let negativos = 0;

for(let i = 0; i < 5; i++) {
    let num = Number(prompt(`Ingrese el número ${i+1}`));
    // Incrementa positivos o negativos según corresponda
}
```

---

## Ejercicio 7: Número primo
**Objetivo:** Practicar bucles anidados y operadores.  
**Enunciado:** Pide un número e indica si es primo o no.

```javascript
let num = Number(prompt("Ingrese un número"));
// Usa un bucle para verificar si es divisible por algún número menor que él
```

---

## Ejercicio 8: Factorial de un número
**Objetivo:** Practicar bucles y operadores de multiplicación.  
**Enunciado:** Pide un número y calcula su factorial usando un bucle `for`.

```javascript
let numero = Number(prompt("Ingrese un número"));
let factorial = 1;
// Calcula el factorial con un bucle
```

---

## Ejercicio 9: Números pares hasta N
**Objetivo:** Practicar bucles y operadores.  
**Enunciado:** Pide un número N e imprime todos los números pares desde 1 hasta N.

```javascript
let N = Number(prompt("Ingrese un número"));
// Usa un bucle y el operador % para imprimir los pares
```

---

## Ejercicio 10: Adivina el número
**Objetivo:** Practicar bucles `while` y condicionales.  
**Enunciado:** El programa genera un número aleatorio entre 1 y 10. El usuario intenta adivinarlo hasta acertar. Indica si su intento es mayor o menor que el número.

```javascript
let numeroSecreto = Math.floor(Math.random() * 10) + 1;
let intento;

while(intento !== numeroSecreto) {
    intento = Number(prompt("Adivina el número entre 1 y 10"));
    // Indica si el intento es mayor, menor o correcto
}
```

---


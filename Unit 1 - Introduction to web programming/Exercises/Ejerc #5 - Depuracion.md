# 📝 Ejercicios de depuración en JavaScript

---

## 1. Error de sintaxis
```js
let nombre = "Ana
console.log(nombre);
```
👉 Problema: El código no se ejecuta.  
✅ Tarea: Encuentra el error y corrígelo.  

---

## 2. Uso incorrecto de variables
```js
console.log(edad);
let edad = 20;
```
👉 Problema: Se produce un error en la consola.  
✅ Tarea: Identifica por qué y corrige el orden del código.  

---

## 3. Operador incorrecto
```js
let a = 5;
let b = 10;
if (a = b) {
  console.log("a es igual a b");
}
```
👉 Problema: El mensaje siempre aparece, aunque `a` no sea igual a `b`.  
✅ Tarea: Corrige el operador de comparación.  

---

## 4. Bucle infinito
```js
let i = 0;
while (i < 5) {
  console.log(i);
}
```
👉 Problema: El bucle no termina.  
✅ Tarea: Identifica el motivo y corrígelo.  

---

## 5. Error en funciones
```js
function saludar() {
  console.log("Hola " + nombre);
}
saludar();
```
👉 Problema: Aparece un error si `nombre` no está definido.  
✅ Tarea: Modifica la función para que reciba `nombre` como parámetro.  

---

## 6. Error en arrays
```js
let frutas = ["manzana", "banana", "pera"];
console.log(frutas[3]);
```
👉 Problema: `undefined` aparece en consola.  
✅ Tarea: Ajusta el código para que no se acceda a un índice fuera del array.  

---

## 7. Error con objetos
```js
let persona = { nombre: "Ana", edad: 25 };
console.log(persona.apellido.toUpperCase());
```
👉 Problema: Se produce un error porque `apellido` no existe.  
✅ Tarea: Corrige el código para que no falle.  

---

## 8. Error en concatenación
```js
let a = 5;
let b = "10";
console.log(a + b);
```
👉 Problema: El resultado no es el esperado (suma numérica).  
✅ Tarea: Convierte correctamente los tipos de datos antes de sumar.  

---

## 9. Error con `if-else`
```js
let nota = 8;
if (nota > 5);
{
  console.log("Aprobado");
} else {
  console.log("Reprobado");
}
```
👉 Problema: Siempre imprime `"Aprobado"`.  
✅ Tarea: Corrige la sintaxis del `if` para que funcione correctamente.  

---

## 10. Mini-reto 🎯
```js
let numeros = [1, 2, 3, 4, 5];
for (let i = 0; i <= numeros.length; i++) {
  console.log(numeros[i]);
}
```
👉 Problema: Aparece `undefined` al final.  
✅ Tarea: Ajusta el bucle para que solo recorra los elementos existentes.

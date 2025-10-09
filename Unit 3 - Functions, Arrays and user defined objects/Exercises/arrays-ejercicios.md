# 🧩 Ejercicios de Arrays en JavaScript

Una recopilación progresiva de ejercicios para practicar **arrays** y sus **métodos más comunes** en JavaScript.

---

## 🟢 Nivel Básico – Fundamentos de Arrays
**Objetivo:** practicar creación, acceso, modificación y recorrido de arrays.

1. **Crear un array** con los nombres de 5 frutas e imprimir la primera y última.  
   - Métodos: `length`, acceso por índice `[ ]`.

2. **Añadir y eliminar elementos** al inicio y al final del array.  
   - Métodos: `push()`, `pop()`, `unshift()`, `shift()`.

3. **Recorrer un array** e imprimir sus elementos.  
   - Métodos: `for`, `for...of`, `forEach()`.

4. **Buscar un elemento** en un array de números.  
   - Métodos: `indexOf()`, `includes()`.

5. **Concatenar arrays** y mostrar el resultado.  
   - Métodos: `concat()`, *spread operator* `...`.

---

## 🟡 Nivel Intermedio – Transformación y Filtrado
**Objetivo:** aprender a transformar, filtrar y ordenar arrays.

6. **Duplicar los valores** de un array numérico.  
   - Método: `map()`.

7. **Filtrar los números pares** de un array.  
   - Método: `filter()`.

8. **Sumar todos los valores** de un array.  
   - Método: `reduce()`.

9. **Ordenar un array de nombres** alfabéticamente y en orden inverso.  
   - Métodos: `sort()`, `reverse()`.

10. **Convertir un array en una cadena de texto** separada por comas.  
    - Método: `join()`.

11. **Dividir una cadena de texto en un array.**  
    - Método: `split()`.

---

## 🔵 Nivel Avanzado – Manipulación y Combinaciones
**Objetivo:** combinar métodos y resolver problemas prácticos.

12. **Eliminar duplicados** de un array.  
    - Métodos: `filter()`, `indexOf()`, o `Set`.

13. **Encontrar el número mayor y menor** en un array.  
    - Métodos: `Math.max()`, `Math.min()`, *spread operator* `...`.

14. **Aplanar un array de arrays.**  
    - Ejemplo: `[[1,2],[3,4]] → [1,2,3,4]`  
    - Método: `flat()`.

15. **Contar cuántas veces aparece un elemento** en un array.  
    - Métodos: `reduce()` o `forEach()`.

16. **Transformar un array de objetos** en un array de una sola propiedad.  
    ```js
    const personas = [
      { nombre: "Ana", edad: 23 },
      { nombre: "Luis", edad: 30 }
    ];
    // Resultado esperado: ["Ana", "Luis"]
    ```
    - Método: `map()`.

17. **Combinar dos arrays** (por ejemplo, de nombres y edades) en uno de objetos.  
    - Método: `map()`.

18. **Ordenar un array de objetos** según una propiedad.  
    ```js
    const usuarios = [
      { nombre: "Ana", edad: 25 },
      { nombre: "Luis", edad: 30 },
      { nombre: "Marta", edad: 20 }
    ];
    usuarios.sort((a, b) => a.edad - b.edad);
    ```

19. **Extraer elementos únicos y ordenarlos** de menor a mayor.  
    - Métodos: `Set`, `sort()`.

20. **Usar chaining de métodos** (`map()`, `filter()`, `reduce()` en cadena).  
    ```js
    const numeros = [1, 2, 3, 4, 5, 6];
    const resultado = numeros
      .filter(n => n % 2 === 0)
      .map(n => n * n)
      .reduce((acc, n) => acc + n, 0);
    console.log(resultado); // 56
    ```

---

## 🧠 Retos de Lógica con Arrays

21. **Revertir manualmente un array** sin usar `reverse()`.  
22. **Comprobar si dos arrays son iguales** (mismos elementos en mismo orden).  
23. **Intercalar elementos** de dos arrays.  
    - Ejemplo: `[1,2,3]` y `["a","b","c"]` → `[1,"a",2,"b",3,"c"]`.
24. **Encontrar el segundo número mayor** en un array.  
25. **Rotar un array** `n` posiciones hacia la derecha o izquierda.  

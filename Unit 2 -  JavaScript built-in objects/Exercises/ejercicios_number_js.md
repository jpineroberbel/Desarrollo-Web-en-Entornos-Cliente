# 📝 Ejercicios con `Number` en JavaScript

## Nivel 1 – Conversión y propiedades básicas
1. **Conversión a número**  
   Convierte las cadenas `"123"`, `"3.14"` y `"abc"` en números usando `Number()`, `parseInt()` y `parseFloat()`. Explica la diferencia en los resultados.

2. **Comprobar si es entero**  
   Escribe una función que reciba un valor y devuelva `true` si es un número entero (`Number.isInteger`) y `false` en caso contrario.

3. **Not a Number**  
   Prueba qué devuelve `Number.isNaN` con los valores: `NaN`, `"hello"`, `undefined`, `0/0`, `parseInt("abc")`.

4. **Valores infinitos**  
   Divide 1 entre 0 y comprueba si el resultado es infinito (`Number.isFinite`).

---

## Nivel 2 – Métodos de instancia
5. **Número con decimales fijos**  
   Dado el número `3.141592`, muéstralo con 2, 4 y 6 decimales usando `.toFixed`.

6. **Representación exponencial**  
   Convierte `123456` a notación científica con `.toExponential(2)`.

7. **Conversión a string con base**  
   Convierte el número `255` a:  
   - Binario  
   - Octal  
   - Hexadecimal  
   usando `.toString(base)`.

8. **Precisión controlada**  
   Usa `.toPrecision` para representar `123.456789` con 4 y 7 cifras significativas.

---

## Nivel 3 – Constantes numéricas
9. **Número máximo y mínimo representable**  
   Muestra los valores de `Number.MAX_VALUE` y `Number.MIN_VALUE`.

10. **Enteros seguros**  
   Verifica si los siguientes números son enteros seguros con `Number.isSafeInteger`:  
   - `9007199254740991`  
   - `9007199254740992`

11. **Epsilon**  
   Demuestra el uso de `Number.EPSILON` comprobando si `0.1 + 0.2` es realmente igual a `0.3`.

---

## Nivel 4 – Retos aplicados
12. **Validador de números**  
   Escribe una función que reciba una cadena y devuelva:  
   - Si es un número válido  
   - Si es entero o decimal  
   - Si es seguro o no  

13. **Formato de precios**  
   Dado un precio `1234.567`, formátalo como:  
   - `1234.57` (2 decimales)  
   - `1.23e+3` (notación científica)  
   - `1235` (redondeado sin decimales)

14. **Generador de binarios aleatorios**  
   Genera un número aleatorio entre 0 y 255 y conviértelo a binario.

15. **Conversión de base genérica**  
   Crea una función que reciba un número y una base (2–36) y lo devuelva representado en esa base con `.toString`.

# 🧩 Retos Avanzados con `Number`, `Math` y `String` en JavaScript

## 🎲 Aleatoriedad avanzada
1. **Generador de matrículas aleatorias**  
   Crea un generador que devuelva matrículas tipo `ABC-1234` con letras y números aleatorios.

2. **Simulador de dados múltiples**  
   Simula lanzar `n` dados de `m` caras. Devuelve un string con los resultados y su suma total.  
   Ejemplo: `3 dados de 6 caras → "4, 2, 6 → total 12"`

3. **Generador de identificadores únicos**  
   Genera un string alfanumérico aleatorio de 16 caracteres usando `Math.random`.

---

## 🧠 Manipulación de Strings compleja

4. **Validador de contraseñas**  
   Escribe una función que valide si una contraseña cumple con:  
   - Al menos 8 caracteres  
   - Una mayúscula  
   - Un número  
   - Un símbolo especial  
   Devuelve un string indicando si es válida o qué reglas no cumple.

5. **Compresor de texto (RLE)**  
   Implementa un compresor de cadenas con **Run-Length Encoding**:  
   - `"aaabbcddd" → "a3b2c1d3"`

6. **Decodificador de texto (RLE)**  
   Haz la función inversa:  
   - `"a3b2c1d3" → "aaabbcddd"`

---

## 🚀 Retos combinados
7. **Juego: adivina el número con intentos limitados**  
   Genera un número aleatorio entre 1 y 100. El usuario tiene 7 intentos. Devuelve mensajes en string indicando si debe subir o bajar, o si ganó.

8. **Generador de tarjetas de crédito falsas**  
   Genera un número de tarjeta válido según el algoritmo de **Luhn**. Devuélvelo como string en el formato `"####-####-####-####"`.

9. **Analizador de dataset en texto**  
   Dado un string con números separados por espacios:  
   `"10 20 30 40 50 60"`  
   Convierte a array de números y calcula:  
   - Promedio  
   - Mediana  
   - Desviación estándar (`Math.sqrt` y fórmulas estadísticas)

10. **Juego de ahorcado simple**  
   Implementa una versión básica del ahorcado con strings:  
   - Palabra oculta como `"javascript"`  
   - Muestra `"j _ v _ s c r i p t"`  
   - Actualiza con cada intento de letra

# Prácticas y Dinámicas de Depuración en JavaScript (JS)

**Objetivo:** Aprender a rastrear el flujo de ejecución, identificar errores lógicos/sintácticos y utilizar las herramientas de desarrollo del navegador (*DevTools*).

---

## Práctica 1: El Inspector de Código (Análisis Estático y Traza)
**Modalidad:** Parejas  
**Herramientas:** Papel/Pizarra + Consola del navegador  

### Descripción
Sin ejecutar el código en el navegador, realiza una traza de ejecución en papel junto a tu compañero. Anota el valor que toma cada variable en cada paso del bucle. Una vez localizado el problema, pruébalo en la consola para confirmar tu hipótesis.

### Reto
Esta función debería recibir un array de números y devolver la suma **únicamente de los números pares**. Sin embargo, no devuelve el resultado correcto o produce comportamientos inesperados.

```javascript
function sumarPares(numeros) {
  let total = 0;
  
  for (let i = 0; i <= numeros.length; i++) {
    if (numeros[i] % 2 = 0) {
      total += numeros[i];
    }
  }
  
  return total;
}

// Prueba de ejecución:
const misNumeros = [2, 7, 4, 11, 8];
console.log("Resultado obtenido:", sumarPares(misNumeros)); 
// Resultado esperado: 14 (2 + 4 + 8)

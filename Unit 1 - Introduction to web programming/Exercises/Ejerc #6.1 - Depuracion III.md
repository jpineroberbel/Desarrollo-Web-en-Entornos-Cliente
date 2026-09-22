# Prácticas y Dinámicas de Depuración en JavaScript (JS)

> **Objetivo:** Aprender a rastrear el flujo de ejecución, identificar errores lógicos/sintácticos y utilizar las herramientas de desarrollo del navegador (*DevTools*).

---

## Práctica 1: El Inspector de Código (Análisis Estático y Traza)
**Modalidad:** Parejas | **Herramientas:** Papel/Pizarra + Consola del navegador  

Sin ejecutar el código en el navegador, realiza una traza de ejecución en papel junto a tu compañero. Anota el valor que toma cada variable en cada paso del bucle. Una vez localizado el problema, pruébalo en la consola para confirmar tu hipótesis.

**Reto:** Esta función debería recibir un array de números y devolver la suma **únicamente de los números pares**. Sin embargo, no devuelve el resultado correcto o produce comportamientos inesperados.

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
```

---

## Práctica 2: Puntos de Interrupción Condicionales y `console.table()`
**Modalidad:** Grupos de 2 o 3 | **Herramientas:** Navegador (Pestaña *Sources* / *Fuente* de DevTools)  

1. Abre las herramientas de desarrollo (*F12* o *Ctrl+Shift+I*).
2. Usa `console.table(carrito)` al inicio para inspeccionar los datos visualmente.
3. Pon un **Breakpoint Condicional** en la línea del bucle para que la ejecución se detenga solo cuando `i === 3` o cuando el precio sea superior a `100`.
4. Inspecciona la pestaña *Scope* (Ámbito) para ver cómo cambian las variables.

```javascript
const carrito = [
  { nombre: "Teclado", precio: "30", aplicarDescuento: false },
  { nombre: "Ratón", precio: 15, aplicarDescuento: true },
  { nombre: "Monitor", precio: 200, aplicarDescuento: true },
  { nombre: "Alfombrilla", precio: 10, aplicarDescuento: false }
];

function calcularTotalCarrito(lista) {
  let total = 0;
  
  for (let i = 0; i < lista.length; i++) {
    let producto = lista[i];
    let precioFinal = producto.precio;

    if (producto.aplicarDescuento) {
      precioFinal = precioFinal - (precioFinal * 0.10); // 10% de descuento
    }

    total = total + precioFinal;
  }

  return total;
}

console.log("Total del carrito:", calcularTotalCarrito(carrito));
// Revisa si el tipo de dato o las operaciones son las correctas.
```

---

## Práctica 3: Caza de Errores (Bug Hunt)
**Modalidad:** Grupos de 3 o 4 | **Herramientas:** Editor de código + DevTools  

Encuentra todos los errores presentes en el código, explica por qué fallan y entrega una versión corregida y funcional.

```javascript
function procesarRegistro(nombre, edadTexto, esEstudiante) {
  // Conversión y validación de edad
  let edad = edadTexto;
  
  if (edad >= 18) {
    let mensajeAcceso = "Acceso concedido a mayores de edad";
  } else {
    let mensajeAcceso = "Acceso restringido a menores";
  }

  console.log(mensajeAcceso);

  // Verificación de descuento por estudiante
  if (esEstudiante = true) {
    console.log("Se ha aplicado el descuento de estudiante.");
  }

  // Recorrido de verificación de historial
  const historialIntentos = [1, 2, 3];
  for (let i = 0; i <= historialIntentos.length; i++) {
    console.log("Verificando intento número: " + historialIntentos[i]);
  }
}

// Caso de prueba
procesarRegistro("Ana", "20", "true");
```

---

## Práctica 4: Lectura de la Pila de Llamadas (*Call Stack*)
**Modalidad:** Individual o Parejas | **Herramientas:** DevTools (Panel *Call Stack*)  

Ejecuta el código en tu navegador. Cuando salte la excepción en la consola, no mires directamente el código: utiliza el depurador para inspeccionar la pila de llamadas e identificar desde qué función se pasó el valor problemático.

```javascript
function calcularPromedio(sumaTotal, cantidad) {
  if (cantidad === 0 || typeof cantidad !== "number") {
    throw new Error("División no válida o cantidad errónea.");
  }
  return sumaTotal / cantidad;
}

function procesarNotasAlumno(notas) {
  let suma = 0;
  for (let i = 0; i < notas.length; i++) {
    suma += notas[i];
  }
  return calcularPromedio(suma, notas.length);
}

function evaluarCandidato(datosAlumno) {
  console.log("Iniciando evaluación de:", datosAlumno.nombre);
  const promedio = procesarNotasAlumno(datosAlumno.notas);
  
  if (promedio >= 5) {
    return "Aprobado";
  } else {
    return "Suspenso";
  }
}

// Simulaciones de prueba:
const alumnoA = { nombre: "Carlos", notas: [6, 8, 5, 7] };
const alumnoB = { nombre: "Elena", notas: [] };

console.log(evaluarCandidato(alumnoA));
console.log(evaluarCandidato(alumnoB)); // ¡Aquí saltará un error!
```

---

## Práctica 5: Depuración con "El Patito de Goma" (*Rubber Duck*)
**Modalidad:** Parejas (Programador y Escuchador)  

1. Un alumno asume el rol de **Programador** y el otro de **Patito de Goma**.
2. El Programador debe explicar en voz alta, línea por línea, qué hace el código y qué valor espera que tenga cada variable.
3. El Patito solo puede escuchar y hacer preguntas aclaratorias. No puede dar la respuesta directa.

```javascript
function esMatrizOrdenada(numeros) {
  let ordenado = true;

  for (let i = 0; i < numeros.length; i++) {
    if (numeros[i] > numeros[i + 1]) {
      ordenado = false;
    }
  }

  return ordenado;
}

console.log(esMatrizOrdenada([1, 3, 5, 8, 12])); // Devuelve false de forma inesperada
console.log(esMatrizOrdenada([4, 2, 9]));       // ¿Funciona correctamente?
```

---

## Práctica 6: Simplificación y Cláusulas de Guarda (*Guard Clauses*)
**Modalidad:** Grupos de 2  

1. Depura el siguiente código para que funcione correctamente según las reglas de negocio.
2. Refactorízalo eliminando los `if` anidados profundos mediante cláusulas de guarda.

```javascript
function validarTransaccion(usuario) {
  let resultado = "";

  if (usuario !== null && usuario !== undefined) {
    if (usuario.activo === true) {
      if (usuario.saldo >= usuario.montoRetiro) {
        if (usuario.montoRetiro > 0) {
          resultado = "Transacción autorizada";
        } else {
          resultado = "Monto inválido";
        }
      } else {
        resultado = "Saldo insuficiente";
      }
    } else {
      resultado = "Usuario inactivo";
    }
  } else {
    resultado = "Usuario no encontrado";
  }

  return resultado;
}

// Caso a probar:
const cliente = { activo: "true", saldo: 100, montoRetiro: 50 };
console.log(validarTransaccion(cliente)); 
```

---

## Guía rápida de atajos para el depurador (*DevTools*)

| Acción | Tecla (Windows/Linux) | Tecla (macOS) | Descripción |
| :--- | :--- | :--- | :--- |
| **Pausar / Reanudar** | `F8` | `Cmd + \` | Continúa la ejecución hasta el siguiente breakpoint. |
| **Paso por encima (*Step Over*)** | `F10` | `Cmd + '` | Ejecuta la siguiente línea sin entrar en funciones. |
| **Paso dentro (*Step Into*)** | `F11` | `Cmd + ;` | Entra dentro de la función que se ejecuta en esa línea. |
| **Paso salir (*Step Out*)** | `Shift + F11` | `Shift + Cmd + ;` | Sale de la función actual y vuelve a la llamadora. |
| **Instrucción `debugger;`** | Escritura directa | Escritura directa | Añade esta palabra en JS para crear un breakpoint por código. |

---

# Relación de Ejercicios: Operadores Lógicos en JavaScript
**Objetivo:** Practicar todos los operadores lógicos (&&, ||, !) usando condicionales y bucles.

---

## Ejercicio 1: Edad y permiso
**Objetivo:** Practicar && (AND).  
**Enunciado:** Pide al usuario su edad y si tiene permiso de sus padres (sí/no). Solo puede entrar si es mayor de 18 y tiene permiso.

```javascript
let edad = Number(prompt("Ingrese su edad"));
let permiso = prompt("¿Tiene permiso de sus padres? (sí/no)");
// Usa un condicional con && para determinar si puede entrar
```

---

## Ejercicio 2: Aprobado en materias
**Objetivo:** Practicar || (OR).  
**Enunciado:** Pide si el alumno aprobó matemáticas, física y química (sí/no). Si aprobó al menos una materia, puede pasar al siguiente nivel.

```javascript
let matematicas = prompt("¿Aprobó matemáticas? (sí/no)");
let fisica = prompt("¿Aprobó física? (sí/no)");
let quimica = prompt("¿Aprobó química? (sí/no)");
// Usa un condicional con || para determinar si pasa al siguiente nivel
```

---

## Ejercicio 3: Contraseña correcta
**Objetivo:** Practicar ! (NOT).  
**Enunciado:** Pide al usuario una contraseña. Si no es correcta, muestra “Contraseña incorrecta”.

```javascript
let contraseña = prompt("Ingrese la contraseña");
// Usa ! para comprobar si no es correcta
```

---

## Ejercicio 4: Número dentro de rango
**Objetivo:** Combinar operadores lógicos.  
**Enunciado:** Pide un número y verifica si está entre 10 y 50 inclusive.

```javascript
let numero = Number(prompt("Ingrese un número"));
// Usa && para verificar el rango
```

---

## Ejercicio 5: Mayoría de edad o tutor presente
**Objetivo:** Practicar combinación de AND y OR.  
**Enunciado:** Pide la edad del usuario y si tiene tutor. Puede entrar si es mayor de 18 o si tiene tutor presente.

```javascript
let edad = Number(prompt("Ingrese su edad"));
let tutor = prompt("¿Tiene tutor presente? (sí/no)");
// Usa && y || según corresponda
```

---

## Ejercicio 6: Verificación de acceso
**Objetivo:** Practicar condiciones múltiples con operadores lógicos.  
**Enunciado:** Pide usuario y contraseña. El acceso es válido si:
- Usuario es “admin” y contraseña es “1234”  
- O usuario es “invitado” y no necesita contraseña

```javascript
let usuario = prompt("Ingrese su usuario");
let contraseña = prompt("Ingrese su contraseña");
// Condicional usando && y ||
```

---

## Ejercicio 7: Números positivos y menores que 100
**Objetivo:** Practicar operadores combinados.  
**Enunciado:** Pide un número e indica si es positivo y menor que 100.

```javascript
let numero = Number(prompt("Ingrese un número"));
// Usa operadores lógicos para evaluar ambas condiciones
```

---

## Ejercicio 8: Día laborable
**Objetivo:** Practicar || con cadenas.  
**Enunciado:** Pide un día de la semana y verifica si es un día laborable (lunes a viernes).

```javascript
let dia = prompt("Ingrese un día de la semana");
// Usa || para comparar con lunes, martes, miércoles, jueves, viernes
```

---

## Ejercicio 9: Votación válida
**Objetivo:** Practicar combinación de operadores.  
**Enunciado:** Pide la edad del votante y su nacionalidad. Puede votar si tiene 18 años o más y es ciudadano del país.

```javascript
let edad = Number(prompt("Ingrese su edad"));
let nacionalidad = prompt("Ingrese su nacionalidad");
// Usa && y >= para verificar la condición
```

---

## Ejercicio 10: Control de acceso con bucle
**Objetivo:** Practicar operadores lógicos dentro de un bucle.  
**Enunciado:** Pide usuario y contraseña hasta que el acceso sea válido (usuario “admin” y contraseña “1234”). Muestra mensaje de error mientras no sea correcto.

```javascript
let usuario, contraseña;

while (!(usuario === "admin" && contraseña === "1234")) {
    usuario = prompt("Usuario:");
    contraseña = prompt("Contraseña:");
    // Mensaje de error si no es correcto
}
console.log("¡Acceso permitido!");
```

---


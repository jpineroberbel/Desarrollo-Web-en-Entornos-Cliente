# Ejercicios de JavaScript: Cookies

## Introducción

En estos ejercicios vamos a trabajar con **cookies en JavaScript**.

Una cookie permite almacenar pequeños datos en el navegador del usuario para poder recuperarlos posteriormente.

Durante los ejercicios aprenderás a:

* Crear cookies.
* Consultar cookies.
* Modificar cookies.
* Eliminar cookies.
* Establecer una fecha de caducidad.
* Utilizar cookies junto con HTML y JavaScript.
* Crear una pequeña aplicación que recuerde información del usuario.


# Ejercicio 1 — Crear una cookie

Crea una cookie llamada `nombre` cuyo valor sea tu nombre.

Después muestra por consola el contenido de:

```javascript
document.cookie
```

### Objetivo

Comprobar cómo se crea una cookie y cómo podemos consultar las cookies almacenadas por nuestra página.

### Comprobación

Abre las herramientas de desarrollador del navegador y busca dónde se almacenan las cookies de la página.

---

# Ejercicio 2 — Crear varias cookies

Crea las siguientes cookies:

```text
nombre = tu nombre
edad = tu edad
ciudad = tu ciudad
```

Después muestra por consola todas las cookies.

El resultado debería ser parecido a:

```text
nombre=Juan; edad=25; ciudad=Granada
```

### Preguntas

1. ¿Cómo aparecen separadas las diferentes cookies?
2. ¿Se muestran en el mismo orden en el que las has creado?
3. ¿Qué ocurre si vuelves a cargar la página?

---

# Ejercicio 3 — Modificar una cookie

Crea inicialmente una cookie:

```text
nombre = Juan
```

Después modifica su valor para que sea:

```text
nombre = Pedro
```

Muestra por consola el resultado final.

### Comprobación

Comprueba en las herramientas de desarrollador que la cookie contiene finalmente:

```text
nombre = Pedro
```

### Pregunta

¿Qué ocurre cuando creamos una cookie utilizando un nombre que ya existe?

---

# Ejercicio 4 — Comprobar la persistencia

Crea una cookie llamada:

```text
usuario = tu nombre
```

Después realiza las siguientes pruebas:

1. Recarga la página.
2. Cierra la pestaña.
3. Vuelve a abrir la página.
4. Cierra completamente el navegador.
5. Vuelve a abrir el navegador y accede de nuevo a la página.

Comprueba en cada caso si la cookie sigue existiendo.

### Pregunta

¿Por qué crees que la cookie sigue existiendo aunque hayas cerrado la página?

---

# Ejercicio 5 — Buscar una cookie

Tenemos las siguientes cookies:

```javascript
document.cookie = "nombre=Juan";
document.cookie = "ciudad=Granada";
document.cookie = "edad=25";
```

`document.cookie` devuelve todas las cookies juntas.

Crea un programa que permita obtener únicamente el valor de la cookie `nombre`.

El resultado debe ser:

```text
Juan
```

### Pista

Puedes utilizar:

```javascript
split()
```

para separar una cadena de texto.

Por ejemplo:

```javascript
let texto = "nombre=Juan; ciudad=Granada; edad=25";

let datos = texto.split(";");
```

Comprueba qué contiene `datos`.

---

# Ejercicio 6 — Crear una función para obtener cookies

Vamos a crear una función que podamos reutilizar para obtener cualquier cookie.

Crea una función:

```javascript
obtenerCookie(nombre)
```

La función debe recibir el nombre de una cookie y devolver su valor.

Por ejemplo:

```javascript
console.log(obtenerCookie("nombre"));
```

debería mostrar:

```text
Juan
```

Y:

```javascript
console.log(obtenerCookie("ciudad"));
```

debería mostrar:

```text
Granada
```

Si la cookie no existe, la función debe devolver:

```javascript
null
```

### Pruebas

Comprueba que funcionan estas llamadas:

```javascript
console.log(obtenerCookie("nombre"));
console.log(obtenerCookie("edad"));
console.log(obtenerCookie("ciudad"));
console.log(obtenerCookie("direccion"));
```

---

# Ejercicio 7 — Guardar el nombre del usuario

Crea una página HTML con:

```text
¿Cuál es tu nombre?

[________________] [Guardar]
```

Cuando el usuario escriba su nombre y pulse **Guardar**:

1. Debes almacenar el nombre en una cookie.
2. Debes mostrar en la página:

```text
¡Hola, Juan!
```

Por ejemplo, si el usuario introduce `Juan`:

```text
¡Hola, Juan!
```

### Requisitos

Debes utilizar:

* Un `<input>`.
* Un `<button>`.
* JavaScript.
* Una cookie.
* Un evento `click`.

---

# Ejercicio 8 — Recuperar el nombre

Modifica el ejercicio anterior.

Cuando se cargue la página:

### Si existe la cookie `nombre`

Debe aparecer:

```text
¡Bienvenido de nuevo, Juan!
```

### Si no existe

Debe aparecer:

```text
No conocemos tu nombre.
```

El programa debe comprobar la existencia de la cookie al cargar la página.

### Prueba

Realiza las siguientes pruebas:

1. Borra las cookies de la página.
2. Abre la página.
3. Comprueba que aparece "No conocemos tu nombre".
4. Introduce tu nombre.
5. Recarga la página.
6. Comprueba que aparece el mensaje de bienvenida.

---

# Ejercicio 9 — Cambiar el nombre

Amplía el ejercicio anterior.

La página debe tener:

```text
Nombre: [________________]

[Guardar nombre]
```

Si el usuario introduce un nombre diferente y pulsa el botón, la cookie debe actualizarse.

Por ejemplo:

Primero:

```text
Nombre: Juan
```

Después:

```text
Nombre: María
```

Al recargar la página debe aparecer:

```text
¡Bienvenida de nuevo, María!
```

---

# Ejercicio 10 — Borrar el nombre

Añade un segundo botón:

```text
[Guardar nombre] [Borrar nombre]
```

El botón **Borrar nombre** debe eliminar la cookie `nombre`.

Después de eliminarla, la página debe mostrar:

```text
No conocemos tu nombre.
```

### Comprobación

Después de pulsar **Borrar nombre**:

1. Comprueba el contenido de `document.cookie`.
2. Comprueba las cookies desde las herramientas de desarrollador.
3. Recarga la página.
4. Comprueba que el nombre ya no aparece.

---

# Ejercicio 11 — Cookie con fecha de caducidad

Hasta ahora nuestras cookies no tenían una fecha de caducidad explícita.

Crea una cookie llamada:

```text
nombre
```

que tenga una duración de **1 día**.

Para calcular fechas puedes utilizar el objeto:

```javascript
Date
```

### Prueba

Comprueba en las herramientas de desarrollador:

* El nombre de la cookie.
* Su valor.
* Su fecha de caducidad.

---

# Ejercicio 12 — Cookie que dura 30 segundos

Modifica el ejercicio anterior para crear una cookie que dure solamente **30 segundos**.

Realiza esta prueba:

1. Crea la cookie.
2. Comprueba que existe.
3. Espera 30 segundos.
4. Recarga la página.
5. Comprueba si sigue existiendo.

### Pregunta

¿Qué ocurre con la cookie cuando supera su fecha de caducidad?

---

# Ejercicio 13 — Miniaplicación: "Bienvenido a mi página"

Crea una pequeña aplicación que recuerde el nombre del usuario.

La primera vez que entre en la página debe aparecer:

```text
¿Cuál es tu nombre?

[________________] [Guardar]
```

Cuando introduzca su nombre:

```text
¡Hola, Juan!
```

El nombre debe almacenarse en una cookie.

---

## Segunda visita

Si el usuario vuelve a entrar en la página y la cookie todavía existe, debe aparecer:

```text
¡Hola de nuevo, Juan!
```

No debe volver a pedirle el nombre.

---

## Cambiar el nombre

Debe existir un botón:

```text
[Cambiar nombre]
```

Al pulsarlo, el usuario podrá introducir un nuevo nombre.

---

## Borrar el nombre

Debe existir también un botón:

```text
[Borrar nombre]
```

Al pulsarlo:

1. Se elimina la cookie.
2. Desaparece el mensaje de bienvenida.
3. Vuelve a aparecer el formulario para introducir el nombre.

---

# Reto final

Añade a la aplicación una cookie llamada:

```text
visitas
```

Cada vez que el usuario visite la página, el contador debe aumentar en uno.

Por ejemplo:

```text
Hola, Juan.

Esta es tu visita número 5.
```

Si el usuario cierra el navegador y vuelve a entrar, el contador debe continuar desde el valor anterior.

### Requisitos

La aplicación final debe utilizar al menos estas dos cookies:

```text
nombre
visitas
```

Y debe permitir:

* Guardar el nombre.
* Recuperar el nombre.
* Modificar el nombre.
* Borrar el nombre.
* Contabilizar las visitas.
* Mantener la información al recargar la página.

---

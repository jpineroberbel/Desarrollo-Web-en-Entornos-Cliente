# Ejercicios básicos de Vue: Interpolación, `v-model` y `v-for`

## 1. Interpolación (`{{ }}`)

1. **Saludo y año:** Crea los datos `nombre` y `anioActual`. Muestra en pantalla: `"Hola, soy [nombre] y estamos en [anioActual]"`.
2. **Operación directa:** Crea `precioBase` y `iva` (por ejemplo `21`). Muestra el precio base, el IVA y el cálculo directo dentro de `{{ }}` (`precioBase + (precioBase * iva) / 100`).
3. **Acceso a un objeto:** Crea un objeto `coche` con `marca`, `modelo` y `kilometros`. Muestra cada dato en un párrafo distinto usando notación de punto.

---

## 2. Enlace bidireccional (`v-model`)

4. **Eco de texto:** Pon un `<input type="text">` con `v-model="mensaje"` y muestra debajo: `Has escrito: {{ mensaje }}`.
5. **Contador de caracteres:** Vincula un `<textarea>` con `v-model="texto"` y muestra: `Longitud: {{ texto.length }}`.
6. **Selector de ciudad:** Crea un `<select>` con 4 ciudades y muestra debajo: `Ciudad elegida: {{ ciudadSeleccionada }}`.
7. **Casilla de confirmación:** Pon un `<input type="checkbox" v-model="acepta">` y muestra al lado: `Estado: {{ acepta }}`.

---

## 3. Listas (`v-for`) y combinación

8. **Lista simple:** Crea un array `frutas = ['Manzana', 'Pera', 'Naranja']` y píntalo como una lista `<ul>` con `<li>` usando `v-for`.
9. **Lista con posición:** Recorre el array `lenguajes = ['HTML', 'CSS', 'JavaScript']` con `v-for="(lenguaje, indice) in lenguajes"` y muestra `1. HTML`, `2. CSS`, etc. (`indice + 1`).
10. **Objetos con `:key`:** Crea un array de objetos `productos` con `id`, `nombre` y `precio`. Pinta cada uno en un `<li>` con `:key="producto.id"` mostrando `{{ producto.nombre }} - {{ producto.precio }} €`.
11. **Editar un dato de la lista:** Usa el array anterior (`productos`) y añade dentro de cada `<li>` un `<input type="number" v-model="producto.precio">` para ver cómo cambia el precio interpolado en la misma fila.
12. **Título dinámico desde input:** Pon un `<input v-model="tituloSeccion">` encima de una lista `v-for` de tareas, de modo que el `<h2>` de la lista cambie al escribir.
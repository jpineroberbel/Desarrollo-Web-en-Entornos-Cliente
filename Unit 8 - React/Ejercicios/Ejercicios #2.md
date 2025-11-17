# Ejercicios de React: Componentes y Estado

## 1. Contador Simple

Este es el "Hola Mundo" del estado de React.

**Objetivo:** Entender el ciclo de vida básico de `useState`: inicializar, leer y actualizar un estado numérico.

**Requisitos:**
* Mostrar un número (que empieza en 0).
* Tener un botón "Incrementar" que suma 1 al número.
* Tener un botón "Decrementar" que resta 1 al número.
* Tener un botón "Resetear" que devuelve el número a 0.

**Conceptos Clave:**
* `useState(0)` para guardar el número.
* Eventos `onClick` en los botones.
* Llamar a `setCount(count + 1)` para actualizar.

**🧩 Desafío Adicional (Bonus):**
* Añade un botón "Duplicar" que multiplique el valor actual por 2.
* Impide que el contador baje de 0 (agregando lógica en el `onClick` de decrementar).

---

## 2. Alternador de Visibilidad (Toggle)

Este ejercicio es fundamental para practicar el renderizado condicional.

**Objetivo:** Usar un estado booleano para mostrar u ocultar un elemento.

**Requisitos:**
* Tener un botón que diga "Mostrar/Ocultar".
* Tener un bloque de texto (un `<p>` con "Lorem ipsum...") que esté visible al inicio.
* Al hacer clic en el botón, el bloque de texto debe desaparecer.
* Al volver a hacer clic, el texto debe reaparecer.

**Conceptos Clave:**
* `useState(true)` para guardar el estado de visibilidad.
* Usar la función de *updater* para invertir el valor: `setIsVisible(prev => !prev)`.
* **Renderizado Condicional** en JSX usando el operador ternario (`isVisible ? <p>...</p> : null`) o un `&&` (`isVisible && <p>...</p>`).

**🧩 Desafío Adicional:**
* En lugar de `null`, muestra un mensaje que diga "El texto está oculto".
* Cambia el texto del botón: si el texto está visible, el botón debe decir "Ocultar"; si está oculto, debe decir "Mostrar".

---

## 3. Sincronizador de Input (Componente Controlado)

Esencial para entender cómo funcionan los formularios en React.

**Objetivo:** Vincular el valor de un campo de texto (`<input>`) al estado de React.

**Requisitos:**
* Tener un campo de texto (`<input type="text">`).
* Tener un párrafo (`<p>`) debajo del input.
* A medida que el usuario escribe en el input, el texto en el párrafo debe replicar exactamente y en tiempo real lo que se está escribiendo.

**Conceptos Clave:**
* `useState("")` para guardar el string del input.
* La prop `value` del input debe estar ligada al estado: `value={texto}`.
* La prop `onChange` del input debe actualizar el estado: `onChange={(e) => setTexto(e.target.value)}`.

**🧩 Desafío Adicional:**
* Añade un botón "Limpiar" que vacíe el input (poniendo el estado en `""`).
* Añade un segundo párrafo que muestre cuántos caracteres se han escrito (ej. "Caracteres: 12"). (Pista: `texto.length`).

---

## 4. Cambiador de Color de Caja

Ideal para ver cómo el estado puede afectar directamente los estilos CSS.

**Objetivo:** Usar el estado para cambiar dinámicamente los estilos de un elemento.

**Requisitos:**
* Mostrar un `<div>` grande que sea un cuadrado (ej. `200px` x `200px`) con un color de fondo inicial (ej. "grey").
* Tener un `<input>` donde el usuario pueda escribir un color (ej. "red", "blue", "#FF00FF").
* El color de fondo del cuadrado debe actualizarse en tiempo real a medida que el usuario escribe en el input.

**Conceptos Clave:**
* `useState("grey")` para guardar el string del color.
* Usar un componente controlado (como en el ejercicio 3) para el input.
* Aplicar estilos en línea (inline styles) dinámicamente: `<div style={{ backgroundColor: color }}>...</div>`.

**🧩 Desafío Adicional:**
* Añade 3 botones ("Rojo", "Verde", "Azul") que, al hacer clic, cambien el color a esos valores predefinidos (actualizando el mismo estado).

---

## 6. Formulario Básico (Múltiples Estados)

Una introducción a cómo manejar múltiples campos de formulario.

**Objetivo:** Manejar múltiples piezas de estado independientes para un formulario.

**Requisitos:**
* Un formulario (`<form>`) con dos inputs: "Nombre" y "Email".
* Un botón "Enviar".
* Al enviar el formulario (hacer clic en el botón), no se debe recargar la página.
* Debajo del formulario, mostrar un mensaje con los datos enviados, ej: "Usuario registrado: Nombre: [nombre], Email: [email]".

**Conceptos Clave:**
* Usar múltiples hooks `useState`:
* Manejar el evento `onSubmit` del formulario.
* Usar `e.preventDefault()` en la función `onSubmit` para evitar la recarga de la página.
* Crear un tercer estado (ej. `userData`) para guardar los datos *enviados* y mostrarlos.

**🧩 Desafío Adicional:**
* En lugar de guardar los datos en otro estado, oculta el formulario después de enviarlo y muestra solo el mensaje de éxito. (Usa un estado booleano `isSubmitted`).

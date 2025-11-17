# Ejercicios de React: Props y Flujo de Datos

El objetivo de estos ejercicios es entender cómo **pasar datos** (unidireccionalmente) de un componente padre a un componente hijo y, lo más importante, cómo **"levantar el estado"** (pasar funciones) para que un hijo pueda modificar el estado de un padre.

---

## 1. Saludo Personalizado (Pasando Strings)

**Objetivo:** Practicar el paso de `props` simples (strings) y ver la reutilización de componentes.

**Requisitos:**
* El componente `App` (Padre) debe renderizar **tres** instancias del componente `Saludo` (Hijo).
* `App` debe pasar una `prop` llamada `nombre` a cada `Saludo` con un valor diferente (ej. "Ana", "Beto", "Carla").
* El componente `Saludo` debe recibir la `prop` y renderizar un mensaje como: "¡Hola, **Ana**!".

**Conceptos Clave:**
* Pasar props en JSX: `<Saludo nombre="Ana" />`.
* Recibir `props` en el componente hijo: `function Saludo(props)` o `function Saludo({ nombre })` (con desestructuración).
* Renderizar el valor de la prop: `{props.nombre}` o `{nombre}`.

**🧩 Desafío Adicional:**
* Añade una segunda prop `emoji` y muéstrala al lado del saludo (ej. "¡Hola, Ana! 👋").

---

## 2. Tarjeta de Perfil (Pasando Múltiples Tipos de Datos)

**Objetivo:** Pasar props de distintos tipos (strings, números, booleanos) y usarlos dentro del hijo para lógica y estilos.

**Requisitos:**
* El componente `App` (Padre) debe renderizar varias tarjetas de `Perfil` (Hijo).
* `App` debe pasar las siguientes props a `Perfil`:
    * `nombre` (string)
    * `edad` (number)
    * `isOnline` (boolean)
    * `imagenUrl` (string, una URL a una imagen de perfil)
* El componente `Perfil` debe:
    * Mostrar la `imagenUrl` en una etiqueta `<img>`.
    * Mostrar el `nombre` y la `edad`.
    * **Renderizado Condicional:** Mostrar un indicador "Online" (ej. un círculo verde) si `isOnline` es `true`, o "Offline" (círculo rojo) si es `false`.

**Conceptos Clave:**
* Pasar múltiples props
* Usar props booleanas para renderizado condicional.
* Usar props para atributos de HTML (como `src` en `<img>`).

**🧩 Desafío Adicional:**
* Si `isOnline` es `false`, aplica un estilo de "escala de grises" (`filter: 'grayscale(100%)'`) a la imagen de perfil.

---

## 3. Lista de Productos (Pasando Arrays)

**Objetivo:** Aprender a pasar un array como prop y cómo el componente hijo debe renderizarlo usando `.map()`.

**Requisitos:**
* En `App` (Padre), define un **array de objetos** que represente productos. Cada objeto debe tener `id`, `nombre` y `precio`.
* Pasa este array completo como una prop `productos` al componente `ListaProductos` (Hijo).
* El componente `ListaProductos` debe recibir el array y usar `.map()` para renderizar la lista.
* Por cada ítem en el map, `ListaProductos` debe renderizar un componente `Producto` (Nieto), pasándole las propiedades de ese producto individual (nombre, precio).
* El componente `Producto` (el nieto) solo se encarga de mostrar el nombre y el precio de *un* producto.

**Conceptos Clave:**
* Pasar un array
* Usar `.map()` sobre una prop de tipo array.
* **Composición:** `App` -> `Lista` -> `Item`.
* Pasar la `key` única a cada elemento en un `.map()` (ej. `key={producto.id}`).

---

## 4. Botón Reutilizable (Levantando el Estado - "Lifting State Up")

Este es el ejercicio **más importante** de esta tanda. Combina `useState` del padre con `props` del hijo.

**Objetivo:** Entender cómo un componente hijo puede modificar el estado de su componente padre pasando funciones como props.

**Requisitos:**
* El componente `ContadorPadre` (Padre) debe tener una variable de estado `count` (iniciada en 0) usando `useState`.
* `ContadorPadre` debe mostrar el valor actual de `count` (ej. `<h1>Contador: {count}</h1>`).
* `ContadorPadre` debe definir una función (ej. `incrementar`) que actualice su propio estado (`setCount(count + 1)`).
* `ContadorPadre` debe renderizar el componente `BotonIncrementar` (Hijo).
* `ContadorPadre` debe pasar su función `incrementar` como una prop al hijo (ej. `<BotonIncrementar onClick={incrementar} />`).
* El componente `BotonIncrementar` (el hijo) **no debe tener estado**. Debe ser un "componente tonto".
* `BotonIncrementar` debe renderizar un `<button>` y asignarle el `onClick` de la prop que recibió.

**Conceptos Clave:**
* **"Lifting State Up"**: El estado vive en el ancestro común (el Padre).
* **Pasar funciones como props:** `onClick={funcionDelPadre}`.
* **Llamar funciones de props:** El hijo ejecuta `props.onClick` sin saber qué hace, solo sabe que es una función.

**🧩 Desafío Adicional:**
* Crea un segundo componente hijo `BotonResetear` que reciba una función del padre para poner el `count` a 0. Ambos hijos modifican el *mismo* estado del padre.

---

## 5. Contenedor Genérico (Usando `props.children`)

**Objetivo:** Entender la prop especial `children` para crear componentes "envoltorio" o contenedores.

**Requisitos:**
* Crea un componente `Card` que renderice un `<div>` con un borde y algo de `padding` (para que parezca una tarjeta).
* El componente `Card` debe aceptar una prop `title` (string) y mostrarla en un `<h2>` dentro de la tarjeta.
* El componente `Card` debe renderizar **`props.children`** debajo del título.
* En `App`, usa el componente `Card` de esta forma:
    ```jsx
    <Card title="Bienvenida">
      <p>Este es el contenido de la primera tarjeta.</p>
      <button>Click aquí</button>
    </Card>
    
    <Card title="Despedida">
      <img src="..." alt="adiós" />
    </Card>
    ```
* Todo lo que `App` pone *dentro* de las etiquetas `<Card>...</Card>` debe aparecer en el lugar donde `Card` renderizó `props.children`.

**Conceptos Clave:**
* `props.children`: Una prop especial que contiene el JSX que se pasa entre las etiquetas de apertura y cierre de un componente.
* Componentes de Composición/Layout.

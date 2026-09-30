# Prácticas de trabajo colaborativo con Git y GitHub

## Introducción

En estas prácticas aprenderéis a utilizar **Git y GitHub para trabajar en equipo** mientras desarrolláis páginas web estáticas utilizando HTML5 y CSS3.

El objetivo principal no es solamente crear las páginas web, sino aprender a trabajar con un flujo de desarrollo colaborativo:

```text
Repositorio
    ↓
Clonar
    ↓
Crear rama
    ↓
Trabajar
    ↓
Commit
    ↓
Push
    ↓
Pull Request
    ↓
Revisión
    ↓
Merge
    ↓
Actualizar main
```

Durante estas prácticas **no se utilizará JavaScript**. El contenido será HTML y CSS estático.

---

# Normas generales

Todas las prácticas se realizarán en grupos de **3 o 4 personas**.

## 1. No trabajar directamente sobre `main`

La rama `main` debe contener siempre una versión funcional del proyecto.

Cada funcionalidad deberá desarrollarse en una rama independiente.

Por ejemplo:

```text
feature/inicio
feature/menu
feature/contacto
```

---

## 2. Los cambios deben llegar a `main` mediante Pull Request

No se deberá hacer directamente:

```bash
git switch main
git merge ...
```

El objetivo es practicar el flujo de trabajo mediante **Pull Requests de GitHub**.

---

## 3. Los commits deben ser descriptivos

Ejemplos adecuados:

```text
Añade sección de contacto
Crea menú principal
Añade información de los artistas
Corrige enlaces de navegación
```

No son adecuados:

```text
cambios
prueba
cosas
aaaa
final
```

---

## 4. Antes de comenzar una nueva tarea

Siempre deberéis actualizar vuestra copia local de `main`:

```bash
git switch main
git pull
```

Después crearéis la nueva rama:

```bash
git switch -c nombre-de-la-tarea
```

---

## 5. Revisión de Pull Requests

El alumno que realiza un Pull Request **no puede aprobar su propio Pull Request**.

Otro integrante del grupo deberá revisarlo.

---

# EJERCICIO 1 — Nuestro equipo

## Objetivo

Realizar vuestro primer proyecto colaborativo utilizando Git y GitHub.

En este ejercicio aprenderéis el flujo básico:

```text
clone → branch → add → commit → push → Pull Request
```

## Proyecto

Crearéis una página web que presente a vuestro equipo.

El repositorio tendrá inicialmente esta estructura:

```text
grupo-web/
│
├── index.html
├── style.css
└── img/
```

**No debéis crear otros archivos ni carpetas.**

El profesor proporcionará el repositorio inicial.

---

## Contenido de la página

La página deberá contener:

### Cabecera

* Nombre del equipo.
* Título del proyecto.

### Presentación

Una breve descripción del grupo.

### Integrantes

Para cada integrante:

* Nombre.
* Breve descripción.
* Aficiones.
* Tecnologías o conocimientos.

Podéis utilizar imágenes o avatares.

### Pie de página

Deberá aparecer el nombre del equipo y el curso.

---

## Organización del trabajo

Todos los integrantes trabajarán sobre:

```text
index.html
```

Cada alumno deberá añadir su propia información dentro de la sección de integrantes.

Por tanto, **todos modificaréis el mismo archivo HTML**.

---

## Trabajo con Git

Cada integrante deberá:

1. Clonar el repositorio.
2. Crear su propia rama.
3. Añadir su información.
4. Realizar al menos un commit.
5. Subir la rama a GitHub.
6. Crear un Pull Request.
7. Revisar el Pull Request de otro compañero.

---

## Entrega

El repositorio deberá contener:

```text
index.html
style.css
img/
```

La rama `main` deberá contener la información de todos los integrantes.

---

# EJERCICIO 2 — Festival de música

## Objetivo

Aprender a repartir diferentes partes de una página entre los integrantes de un equipo.

## Proyecto

Crearéis una página web estática para un festival de música ficticio.

La estructura será:

```text
festival/
│
├── index.html
├── style.css
└── img/
```

**Solo habrá un archivo HTML.**

---

## Estructura de `index.html`

La página deberá contener las siguientes secciones:

```text
<header>
    Cabecera y menú
</header>

<main>

    <section id="inicio">
    </section>

    <section id="artistas">
    </section>

    <section id="programacion">
    </section>

    <section id="entradas">
    </section>

    <section id="contacto">
    </section>

</main>

<footer>
</footer>
```

---

## Reparto del trabajo

En un grupo de cuatro personas:

| Alumno   | Sección             |
| -------- | ------------------- |
| Alumno 1 | Inicio              |
| Alumno 2 | Artistas            |
| Alumno 3 | Programación        |
| Alumno 4 | Entradas y contacto |

Si el grupo tiene tres integrantes, deberéis repartir las cinco secciones entre los tres.

---

## Contenido mínimo

### Inicio

* Nombre del festival.
* Fecha.
* Lugar.
* Descripción.

### Artistas

Al menos cuatro artistas o grupos.

### Programación

Crear una tabla con:

* Hora.
* Artista.
* Escenario.

### Entradas

Información sobre diferentes tipos de entrada.

### Contacto

Información de contacto y enlaces.

---

## Trabajo con Git

Cada integrante deberá trabajar en una rama diferente:

```text
feature/inicio
feature/artistas
feature/programacion
feature/entradas
```

Cada funcionalidad deberá incorporarse mediante Pull Request.

---

# EJERCICIO 3 — Restaurante

## Objetivo

Practicar el trabajo simultáneo sobre un mismo archivo y aprender a respetar las zonas de trabajo de otros compañeros.

## Proyecto

Crearéis una página web para un restaurante ficticio.

La estructura será:

```text
restaurante/
│
├── index.html
├── style.css
└── img/
```

---

## Estructura de la página

El archivo `index.html` deberá contener:

```text
<header>
    Menú de navegación
</header>

<main>

    <section id="inicio">
    </section>

    <section id="menu">
    </section>

    <section id="restaurante">
    </section>

    <section id="reservas">
    </section>

</main>

<footer>
</footer>
```

---

## Reparto

| Alumno   | Trabajo        |
| -------- | -------------- |
| Alumno 1 | Inicio         |
| Alumno 2 | Menú           |
| Alumno 3 | El restaurante |
| Alumno 4 | Reservas       |

Todos trabajaréis sobre:

```text
index.html
```

---

## Requisito adicional

Todos los integrantes deberán modificar también el menú de navegación.

Cada uno deberá añadir al menú un enlace hacia su sección.

Por tanto, habrá varios alumnos modificando la misma zona del documento.

---

## Objetivo Git

Debéis comprobar qué ocurre cuando varias ramas parten de una misma versión del archivo y realizan cambios diferentes.

Si Git consigue combinar los cambios automáticamente, comprobad el resultado.

Si aparece un conflicto, resolvedlo siguiendo las indicaciones del profesor.

---

# EJERCICIO 4 — Videojuego

## Objetivo

Aprender a identificar y resolver un conflicto de Git.

## Proyecto

Crearéis la página web de un videojuego ficticio.

La estructura será:

```text
videojuego/
│
├── index.html
├── style.css
└── img/
```

---

## Secciones

La página deberá contener:

* Historia.
* Personajes.
* Escenarios.
* Galería.
* Noticias.

---

## Reparto

| Alumno   | Sección            |
| -------- | ------------------ |
| Alumno 1 | Historia           |
| Alumno 2 | Personajes         |
| Alumno 3 | Escenarios         |
| Alumno 4 | Galería y noticias |

Todos trabajarán sobre:

```text
index.html
```

---

## Conflicto intencionado

Todos los integrantes deberán modificar el menú de navegación.

Cada uno deberá añadir al menú el enlace correspondiente a su sección.

Por ejemplo:

```text
Historia
Personajes
Escenarios
Galería
Noticias
```

No intentéis evitar el conflicto.

El objetivo de esta práctica es **aprender a resolverlo**.

---

## Cuando aparezca un conflicto

Deberéis:

1. Identificar el archivo afectado.
2. Abrir el archivo.
3. Localizar las marcas de conflicto.
4. Comprender qué cambios ha realizado cada compañero.
5. Decidir qué contenido debe conservarse.
6. Eliminar las marcas de conflicto.
7. Comprobar que el HTML funciona correctamente.
8. Realizar el commit correspondiente.
9. Continuar con el Pull Request.

---

## Documentación

Añadid al `README.md` una pequeña explicación:

```text
¿Qué conflicto apareció?

¿Qué archivo estaba afectado?

¿Qué cambios había realizado cada persona?

¿Cómo se resolvió?

¿Quién realizó la resolución?
```

---

# EJERCICIO 5 — Agencia de viajes

## Objetivo

Introducir el trabajo colaborativo sobre un archivo CSS compartido.

Hasta ahora habéis trabajado principalmente con HTML. En esta práctica todos colaboraréis también sobre `style.css`.

---

## Proyecto

Crearéis una web para una agencia de viajes.

Estructura:

```text
agencia/
│
├── index.html
├── style.css
└── img/
```

---

## Secciones

El HTML deberá contener:

* Inicio.
* Destinos.
* Ofertas.
* Alojamientos.
* Contacto.

---

## Reparto

| Alumno   | HTML     | CSS        |
| -------- | -------- | ---------- |
| Alumno 1 | Inicio   | Cabecera   |
| Alumno 2 | Destinos | Tarjetas   |
| Alumno 3 | Ofertas  | Botones    |
| Alumno 4 | Contacto | Formulario |

---

## Condición

Todos utilizaréis:

```text
style.css
```

No está permitido crear un CSS diferente para cada alumno.

Antes de comenzar, el grupo deberá acordar:

* Tipografía.
* Tamaños de títulos.
* Colores.
* Diseño de botones.
* Márgenes.
* Espaciado.
* Estilo general.

---

## Objetivo

Comprobar cómo se puede trabajar sobre un archivo compartido y cómo Git permite integrar los cambios realizados por diferentes personas.

---

# EJERCICIO 6 — Revista digital

## Objetivo

Aprender a dividir un proyecto en diferentes archivos para reducir conflictos.

## Proyecto

Crearéis una revista digital.

La estructura será:

```text
revista/
│
├── index.html
├── tecnologia.html
├── videojuegos.html
├── cine.html
├── musica.html
│
├── css/
│   └── style.css
│
└── img/
```

---

## Reparto

Cada integrante será responsable de una página.

| Alumno   | Página           |
| -------- | ---------------- |
| Alumno 1 | tecnologia.html  |
| Alumno 2 | videojuegos.html |
| Alumno 3 | cine.html        |
| Alumno 4 | musica.html      |

La página `index.html` será responsabilidad de todo el grupo.

---

## Cada página deberá contener

* Título.
* Introducción.
* Al menos tres artículos.
* Imágenes.
* Listas.
* Enlaces.
* Una sección de destacados.

---

## Diseño común

Todas las páginas deberán utilizar:

```text
css/style.css
```

También deberán compartir:

* Menú de navegación.
* Estructura de cabecera.
* Pie de página.
* Tipografía.
* Estilo visual.

---

## Objetivo Git

Comprobar las ventajas de repartir el trabajo en archivos independientes.

Cada alumno trabajará principalmente sobre un archivo diferente.

---

# EJERCICIO 7 — Portal turístico con Issues

## Objetivo

Utilizar GitHub no solamente para almacenar código, sino también para **organizar el trabajo de un equipo**.

## Proyecto

Crearéis un portal turístico sobre Andalucía.

La estructura será:

```text
andalucia/
│
├── index.html
├── granada.html
├── cordoba.html
├── sevilla.html
├── malaga.html
│
├── css/
│   └── style.css
│
└── img/
```

---

## Antes de programar

El grupo deberá crear Issues en GitHub.

Como mínimo:

```text
Crear página principal
Crear página de Granada
Crear página de Córdoba
Crear página de Sevilla
Crear página de Málaga
Crear menú de navegación
Crear pie de página
Revisar enlaces
Revisar diseño
```

Cada Issue deberá estar asignada a un integrante.

---

## Flujo obligatorio

Para cada tarea:

```text
Issue
  ↓
Asignación
  ↓
Crear rama
  ↓
Desarrollar
  ↓
Commit
  ↓
Push
  ↓
Pull Request
  ↓
Revisión
  ↓
Merge
```

---

## Requisito

Cada alumno deberá completar al menos **dos Issues**.

Cada alumno deberá realizar al menos:

* 2 ramas.
* 2 commits.
* 2 Pull Requests.
* 2 revisiones de Pull Requests de compañeros.

---

# EJERCICIO 8 — Proyecto final colaborativo

## Objetivo

Aplicar todo lo aprendido en un proyecto web completo.

En este ejercicio podréis elegir libremente la temática.

Algunas posibilidades:

* Restaurante.
* Festival de música.
* Equipo deportivo.
* Videojuego.
* Agencia de viajes.
* Tienda.
* Museo.
* Empresa tecnológica.
* Evento cultural.
* Portal turístico.

---

# Requisitos del proyecto

La web deberá tener como mínimo:

* Página principal.
* Tres páginas adicionales.
* Menú de navegación.
* Cabecera.
* Pie de página.
* Hoja de estilos CSS externa.
* Imágenes.
* Enlaces internos.
* Enlaces externos.
* Listas.
* Al menos una tabla.
* Al menos un formulario.
* HTML5 semántico.
* Diseño responsive básico.

---

# Estructura mínima

La estructura será:

```text
proyecto/
│
├── index.html
│
├── pages/
│   ├── pagina1.html
│   ├── pagina2.html
│   └── pagina3.html
│
├── css/
│   └── style.css
│
└── img/
```

Podéis crear más páginas si el proyecto lo necesita.

---

# Organización del equipo

Antes de comenzar a programar deberéis decidir:

1. Temática del proyecto.
2. Páginas que tendrá.
3. Responsable de cada página.
4. Elementos comunes.
5. Estructura de carpetas.
6. Diseño visual.
7. Tareas que se convertirán en Issues.

---

# GitHub

El proyecto deberá utilizar:

* Repositorio GitHub.
* Rama `main`.
* Ramas de funcionalidades.
* Issues.
* Commits.
* Push.
* Pull Requests.
* Revisión de código.
* Merge.
* Resolución de conflictos.

---

# Requisitos individuales

Cada integrante deberá realizar como mínimo:

* 3 ramas.
* 3 commits.
* 3 Pull Requests.
* 3 revisiones de compañeros.
* 1 resolución de conflicto.

---

# README.md

El repositorio deberá incluir un archivo:

```text
README.md
```

En él se indicará:

## Nombre del proyecto

Nombre de la web.

## Integrantes

Lista de componentes del grupo.

## Descripción

Breve descripción del proyecto.

## Organización

Explicación de cómo se ha repartido el trabajo.

## Git y GitHub

Indicar:

* Número de ramas utilizadas.
* Número aproximado de Pull Requests.
* Conflictos encontrados.
* Cómo se resolvieron.

---

# Checklist antes de entregar

Antes de entregar el proyecto comprobad:

### Web

* [ ] Todas las páginas funcionan.
* [ ] Todos los enlaces funcionan.
* [ ] Las imágenes se muestran correctamente.
* [ ] Todas las páginas utilizan el CSS común.
* [ ] El diseño es coherente.
* [ ] No existen errores evidentes de HTML.
* [ ] La web se visualiza correctamente en ordenador y móvil.

### Git

* [ ] `main` contiene la versión final.
* [ ] No se ha trabajado directamente sobre `main`.
* [ ] Se han utilizado ramas.
* [ ] Los commits tienen mensajes descriptivos.
* [ ] Se han realizado Pull Requests.
* [ ] Los Pull Requests han sido revisados.
* [ ] Se han utilizado Issues.
* [ ] Se ha resuelto al menos un conflicto.

### Repositorio

* [ ] La estructura de carpetas es correcta.
* [ ] No hay archivos innecesarios.
* [ ] No hay archivos duplicados.
* [ ] Existe `README.md`.
* [ ] Todos los integrantes aparecen como colaboradores.
* [ ] El repositorio contiene la versión final del proyecto.

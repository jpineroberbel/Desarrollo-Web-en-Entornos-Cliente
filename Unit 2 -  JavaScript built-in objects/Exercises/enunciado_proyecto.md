# 📝 Enunciado del Proyecto: Reloj Digital con Eventos

## 🎯 Objetivo

El objetivo de este mini-proyecto es **practicar el uso del objeto
`Date` en JavaScript**, comprendiendo cómo trabajar con fechas y horas
en tiempo real, además de cómo comparar fechas para gestionar eventos.

------------------------------------------------------------------------

## 📌 Descripción

Vas a desarrollar una aplicación web sencilla que muestre un **reloj
digital en vivo** y permita al usuario **agregar eventos** (con fecha y
hora).\
Cuando llegue el momento de un evento, la aplicación deberá mostrar un
**aviso en pantalla**.

------------------------------------------------------------------------

## 📂 Requisitos

1.  **Mostrar la hora actual en tiempo real**, actualizándose cada
    segundo.
2.  **Mostrar la fecha actual** en un formato legible (ejemplo: *lunes,
    25 de septiembre de 2025*).
3.  Permitir al usuario **agregar eventos** indicando:
    -   Nombre del evento.
    -   Fecha y hora del evento.
4.  **Listar los eventos futuros** en pantalla.
5.  Cuando llegue la hora de un evento, mostrar un **mensaje de alerta**
    avisando al usuario.

------------------------------------------------------------------------

## 🔧 Pistas técnicas

-   Usa el objeto `Date` y sus métodos principales:
    -   `new Date()`
    -   `getHours()`, `getMinutes()`, `getSeconds()`
    -   `toLocaleDateString()` y `toLocaleString()`
-   Usa `setInterval()` para actualizar el reloj cada segundo.
-   Para comparar fechas, puedes restar dos objetos `Date` y comprobar
    la diferencia en milisegundos.
-   Diseña la interfaz con HTML y CSS para que sea clara y atractiva.

------------------------------------------------------------------------

## ✅ Entregable

-   Un archivo **ZIP** con los tres ficheros:
    -   `index.html`\
    -   `style.css`\
    -   `script.js`

------------------------------------------------------------------------

## ⭐ Retos adicionales (opcionales)

-   Guardar los eventos en **localStorage** para que no se pierdan al
    recargar la página.\
-   Permitir eliminar eventos de la lista.\
-   Personalizar el diseño del reloj con estilos más creativos.

# 🧩 Ejercicios de Eventos en JavaScript

Estos ejercicios están diseñados para manejar **eventos en JavaScript**, sin usar todavía creación dinámica de contenido con el DOM.  
Cada minijuego tiene una **interfaz HTML estática** y los eventos controlan su comportamiento.

---

## 🧱 Nivel 1: Eventos básicos (click, mouseover, keydown)

### 1. Caza del color
**Objetivo:** Hacer clic en el cuadrado del color indicado.  
**Interfaz:** 4 cuadrados de colores (HTML estático).  
**JS:** Mostrar el texto “Haz clic en el color rojo”.  
- Si se hace clic en el color correcto → mensaje de acierto.  
- Si se falla → mensaje de error.  
**Eventos:** `click`

---

### 2. El botón cambiante
**Objetivo:** Un botón cambia de color o texto al pasar el ratón o hacer clic.  
**Interfaz:** Un solo botón grande.  
**JS:**  
- `mouseover`: cambia de color.  
- `mouseout`: vuelve a su color original.  
- `click`: cambia su texto (“¡Me hiciste clic!”).  
**Eventos:** `mouseover`, `mouseout`, `click`

---

### 3. Sigue la instrucción
**Objetivo:** Responder con el teclado a una instrucción.  
**Interfaz:** Texto que dice: “Presiona la tecla A”.  
**JS:** Detectar la tecla presionada y mostrar si fue la correcta.  
**Eventos:** `keydown`

---

## 🎮 Nivel 2: Reacción y precisión

### 4. Juego de reflejos
**Objetivo:** Hacer clic en el círculo solo cuando cambie de color.  
**Interfaz:** Un círculo centrado.  
**JS:**  
- Cada 2–5 segundos el círculo cambia de gris a verde.  
- Si el usuario hace clic cuando está verde → “¡Reflejos rápidos!”.  
- Si hace clic antes → “Demasiado pronto”.  
**Eventos:** `click`, `setTimeout`

---

### 5. Atrapa el número correcto
**Objetivo:** Elegir el número que diga el texto.  
**Interfaz:** Varios botones numerados del 1 al 9.  
**JS:**  
- Mostrar “Haz clic en el número 7”.  
- Validar el número presionado.  
**Eventos:** `click`

---

## 🕹️ Nivel 3: Coordinación y secuencias

### 6. Simón dice (versión simple)
**Objetivo:** Repetir una secuencia de colores.  
**Interfaz:** 4 botones de colores.  
**JS:**  
- Mostrar un color que “parpadea”.  
- El usuario debe hacer clic en ese color.  
- Si acierta, pasa al siguiente nivel.  
**Eventos:** `click`, `setTimeout`

---

### 7. Carrera de botones
**Objetivo:** Pulsar repetidamente un botón para “avanzar” una barra.  
**Interfaz:**  
- Un botón “Correr”.  
- Una barra de progreso (`div` con ancho variable).  
**JS:** Cada clic aumenta el ancho de la barra un poco.  
**Eventos:** `click`

---
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/98b55c32-4ba4-493a-b212-ad8eb296b0fb" />

---

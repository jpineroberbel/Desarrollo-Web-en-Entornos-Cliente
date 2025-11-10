# 🧱 Proyecto: Arkanoid DOM

## 🎯 Objetivo general
Desarrollar un mini juego tipo **Arkanoid / Breakout** utilizando **HTML, CSS y JavaScript**, donde el jugador controla una barra para rebotar una pelota que destruye bloques en pantalla.

El objetivo del jugador es **romper todos los bloques sin dejar que la pelota caiga**.

---

## 🧩 Requisitos funcionales

1. **Área de juego**
   - Debe existir un contenedor `<div>` que represente el escenario del juego.
   - Dentro del contenedor se mostrarán:
     - La **pelota** (elemento circular).
     - La **barra del jugador** (rectángulo).
     - Los **bloques** (múltiples elementos organizados en filas).

2. **Movimiento del jugador**
   - La barra se mueve horizontalmente usando las **teclas de flecha izquierda y derecha**.
   - La barra no puede salir del área del juego.

3. **Movimiento de la pelota**
   - La pelota se mueve automáticamente al iniciar el juego.
   - Rebota en los bordes del contenedor y en la barra.
   - Si la pelota toca el borde inferior, el jugador **pierde una vida o el juego termina**.

4. **Colisión con bloques**
   - Cuando la pelota toca un bloque:
     - El bloque desaparece (se elimina del DOM o se cambia su clase).
     - La pelota rebota.
     - Se suman puntos al marcador.

5. **Marcador**
   - Muestra la cantidad de puntos o bloques destruidos.
   - Opcional: mostrar vidas restantes.

6. **Condiciones de victoria o derrota**
   - El jugador **gana** al destruir todos los bloques.
   - El jugador **pierde** si la pelota toca el borde inferior.

---

## ⚙️ Requisitos técnicos (DOM y JS)

- Usar **JavaScript puro (sin librerías externas)**.
- Manipular elementos del DOM para:
  - Crear y eliminar bloques dinámicamente.
  - Actualizar el marcador.
  - Controlar la posición de la pelota y la barra.
- Detectar colisiones mediante coordenadas (`getBoundingClientRect()` o `offsetTop`, `offsetLeft`).
- Usar `requestAnimationFrame()` o `setInterval()` para el bucle principal del juego.

---

## 🎨 Interfaz sugerida

### Estructura de archivos


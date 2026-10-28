# Ejercicios Prácticos: Eventos de Toque en JavaScript

Esta es una lista de progresión para dominar los eventos de toque (`touchstart`, `touchmove`, `touchend` y `touchcancel`) en la web.

## Nivel Básico e Intermedio

### 1. El Área Sensible (Eventos básicos)
Crea un `div` grande en el centro de la pantalla. Cambia su color de fondo dependiendo del evento: 
* Verde al tocarlo (`touchstart`).
* Amarillo mientras arrastras el dedo dentro de él (`touchmove`).
* Rojo al soltarlo (`touchend`).
* **Extra:** Muestra las coordenadas X e Y actuales del toque dentro del texto del `div`.

### 2. El Círculo Perseguidor (Coordenadas continuas)
Dibuja un círculo (un `div` con `position: absolute` y `border-radius: 50%`). Haz que el centro de este círculo siga exactamente la posición de tu dedo mientras lo arrastras por toda la pantalla, leyendo las propiedades `e.touches[0].clientX` y `clientY`.

### 3. Detector de Deslizamiento (Gestos Swipe)
Crea un bloque de texto en pantalla. Guarda las coordenadas iniciales en el evento `touchstart` y compáralas con las coordenadas finales en el `touchend`. Calcula la diferencia matemática para detectar si el usuario deslizó el dedo hacia la izquierda, derecha, arriba o abajo, y muestra una alerta con la dirección detectada.

### 4. Pinch to Zoom (Multi-touch)
Crea un contenedor con una imagen. Detecta cuando el usuario toca la pantalla con dos dedos comprobando que `e.touches.length === 2`. Calcula la distancia entre ambos puntos en tiempo real durante el evento `touchmove`. Si la distancia aumenta respecto al toque inicial, aplica una propiedad CSS `transform: scale()` para agrandar la imagen; si disminuye, redúcela.

---

## Nivel Avanzado

### 5. Toque Prolongado y Doble Toque (Gestos de tiempo)
Crea un botón en pantalla que responda a interacciones basadas en tiempo:
* **Doble Toque:** Si lo tocas dos veces en menos de 300 milisegundos, cambia su forma a un círculo.
* **Toque Prolongado (Long Press):** Si mantienes el dedo presionado sobre él durante más de 1 segundo sin moverlo, haz que aparezca un menú contextual oculto. 
* *Pista:* Deberás gestionar temporizadores usando `setTimeout` al inicio del toque y cancelarlos con `clearTimeout` en los eventos `touchend` o `touchmove`.

### 6. Carrusel Magnético (Deslizamiento continuo)
Crea una fila horizontal de tarjetas que desborde el ancho de la pantalla. Usa `touchstart` y `touchmove` para mover el contenedor hacia los lados siguiendo el dedo del usuario. Al soltar (`touchend`), calcula la posición actual y aplica una transición CSS para que la tarjeta más cercana se deslice automáticamente hasta el centro de la pantalla (efecto *snap*), imitando el comportamiento nativo de las galerías móviles.

### 7. Zonas de Caída (Touch Drag & Drop)
Dibuja un círculo arrastrable y dos "cajas" vacías en diferentes partes de la pantalla. Arrastra el círculo con `touchmove`. El reto principal ocurre en el `touchend`: a diferencia del ratón, los eventos de toque no detectan por defecto sobre qué elemento estás soltando el dedo. 
* *Pista:* Deberás usar el método `document.elementFromPoint(x, y)` pasándole las coordenadas del toque final para detectar si debajo hay una caja en ese instante exacto, y si es así, acoplar el círculo en su interior.

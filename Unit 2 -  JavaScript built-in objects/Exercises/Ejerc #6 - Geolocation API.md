# Ejercicios para practicar la Geolocation API en JavaScript

Una lista progresiva de ejercicios para aprender a trabajar con la Geolocation API.

---

## 🔹 Nivel Básico

1. **Obtener tu ubicación actual (latitud y longitud)**
   - Usar `navigator.geolocation.getCurrentPosition`.
   - Mostrar las coordenadas en consola.

2. **Mostrar la ubicación en la página**
   - Obtener latitud y longitud.
   - Insertarlas en el DOM dentro de un `<p>`.

3. **Manejo de errores**
   - Implementar `onError` en `getCurrentPosition`.
   - Mostrar mensajes si el usuario deniega permisos o si ocurre un error.

---

## 🔹 Nivel Intermedio

4. **Actualizar ubicación en tiempo real**
   - Usar `navigator.geolocation.watchPosition`.
   - Mostrar en la página cómo cambian las coordenadas al moverte.

5. **Integración con Google Maps o Leaflet**
   - Mostrar tu ubicación en un mapa interactivo con un marcador.
   - El mapa debe actualizarse cuando cambies de posición (con `watchPosition`).

6. **Mostrar precisión de la ubicación**
   - Mostrar en pantalla el valor de `coords.accuracy`.

7. **Calcular la distancia entre dos ubicaciones**
   - Guardar dos pares de coordenadas (tu ubicación y otra fija).
   - Implementar una función que use la fórmula de Haversine para calcular la distancia.

---

## 🔹 Nivel Avanzado

8. **Trazar ruta en un mapa**
   - Usar Leaflet o Google Maps.
   - Dibujar una polilínea con tus posiciones registradas por `watchPosition`.

9. **Geofencing básico**
   - Definir un área (círculo en el mapa).
   - Detectar si entras o sales de esa área según tu posición.

10. **App de rastreo de actividad**
   - Guardar posiciones periódicamente en un array.
   - Calcular distancia recorrida y tiempo transcurrido.
   - Mostrar resultados en pantalla.

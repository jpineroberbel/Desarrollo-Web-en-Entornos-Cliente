# 📝 Ejercicios con `Date` en JavaScript

## Nivel 1 – Creación y lectura de fechas
1. **Fecha actual**  
   Crea un objeto `Date` que represente la fecha y hora actual.

2. **Fecha específica**  
   Crea un objeto `Date` con tu fecha de nacimiento (año, mes, día).

3. **Obtener partes de una fecha**  
   Dado un objeto `Date`, muestra:  
   - Año (`getFullYear`)  
   - Mes (`getMonth`)  
   - Día (`getDate`)  
   - Día de la semana (`getDay`)  
   - Hora, minutos y segundos (`getHours`, `getMinutes`, `getSeconds`)

4. **Convertir a string**  
   Muestra la fecha actual en formato legible usando `.toDateString()` y `.toTimeString()`.

---

## Nivel 2 – Operaciones con fechas
5. **Sumar días**  
   Escribe una función que reciba una fecha y un número de días, y devuelva la nueva fecha resultante.

6. **Diferencia entre dos fechas**  
   Calcula cuántos días faltan desde hoy hasta el próximo 31 de diciembre.

7. **Comparar fechas**  
   Dadas dos fechas, determina cuál es anterior y cuál posterior.

8. **Primer día del mes**  
   Crea una función que, dado un año y un mes, devuelva qué día de la semana fue el primer día de ese mes.

---

## Nivel 3 – Formateo y zonas horarias
9. **ISO string**  
   Convierte la fecha actual a formato ISO (`.toISOString()`).

10. **Fecha local y UTC**  
   Muestra la misma fecha en hora local y en UTC.

11. **Formateo personalizado**  
   Escribe una función que reciba un objeto `Date` y devuelva un string con el formato:  
   `DD/MM/YYYY HH:mm:ss`

12. **Internacionalización**  
   Usa `Intl.DateTimeFormat` para mostrar la fecha actual en:  
   - Español (España)  
   - Inglés (EE.UU.)  
   - Japonés

---

## Nivel 4 – Retos aplicados
13. **Cuenta atrás**  
   Crea un programa que muestre en consola los días, horas, minutos y segundos que faltan para Año Nuevo.

14. **Edad exacta**  
   Escribe una función que reciba una fecha de nacimiento y calcule la edad exacta en años, meses y días.

15. **Calendario simple**  
   Genera un array con todas las fechas de un mes específico (ej. septiembre 2025).

16. **Próximo viernes 13**  
   Escribe un programa que encuentre la próxima fecha que sea viernes 13.

## Notas Recordatorio en VueJS

El presente ejercicio consiste en el desarrollo de una aplicación web mediante VueJS. El alumno/a puede decidir las partes a desarrollar y según ello vendrá determinada la nota final.

![Esta es una imagen de ejemplo](https://www.iesayala.com/moodle/pluginfile.php/8200/mod_page/content/7/Captura%20de%20pantalla_2019-01-21_22-31-07.png)

Contenido Mínimo.

Se pretende desarrollar una aplicación para gestionar recordatorios. El proyecto debe ser puesto en producción. La interfaz debe ser un clon de la siguiente:
Para el desarrollo de la aplicación deben desarrollarse 2 componentes. Un componente para el pie y otro para gestionar la lista de notas. Éste último integra desde el input hasta el pie de página.

Requisitos:
- Todas las notas se guardan en LocalStorage y se leen de ahí al iniciar la aplicación.
- Debe mostrarse el mensaje con el número de tareas pendientes y el total.
- Deben borrarse todas las tareas completadas al pulsar en el link correspondiente.
- Al escribir en el input y pulsar Enter, debe crearse una nota nueva.
- Cada nota debe tener un texto, una prioridad (Low, Normal, High) y un tiempo de creación.
- Para cada nota es posible cambiar su prioridad pulsando en el botón de la nueva prioridad.
- Para cada nota es posible cambiar su estado (completada o no) pulsando en el círculo de la izquierda.
- Para cada nota es posible borrarla pulsando en el botón de la derecha.
- Debe aplicarse el estilo apreciado en la imagen para las tareas ya realizadas.
- Al crearse cada nota debe realizarse una animación.
- Las notas se muestran ordenadas por prioridad (de más alta a más baja), de modo que al cambiar ésta se reordenan automáticamente.
- La aplicación debe organizarse como mínimo en los siguientes componentes: cabecera, pie, contenido y nota
- El realizar todos los apartados anteriores de un modo correcto supondrá un 5 en la nota final del proyecto. La nota podrá llegar hasta 10 según se desarrollen los siguientes apartados con su valoración correspondiente:

- (2 puntos) El proyecto se desarrolla utilizando como generador a vue-cli y adecuando la organización del código y componentes a esta plantilla.
- (1 punto) Añade un input para filtrar las tareas según empiecen por el texto introducido en el nuevo input (filtrar tareas).
- (2 puntos) Se añade  un menú superior con 2 rutas: Notas y El tiempo. Por defecto la aplicación muestra las notas (/) mientras que al pulsar el tiempo se muestra una página para el tiempo (/tiempo). Ésta última será un componente que maquete de un modo sencillo el tiempo actual, obtenido de alguna API REST,  para la ciudad desde la que se carga la web. Esta información se refresca cada 10 minutos.

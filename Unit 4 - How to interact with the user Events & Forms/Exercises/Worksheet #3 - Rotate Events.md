## Eventos de Rotación

Una vez probados los eventos de rotación, vamos a crear una nueva web que tan sólo contendrá un DIV rectangular con un color de fondo. Para ello crea un repositorio en GitHub, linkalo con tu repositorio en local y actívale Pages, de modo que cada cambio que quieras probar, haces un push y ya puedes acceder a la web a través de tu móvil.

a) En primer lugar debes capturar los eventos de rotación y utlizando el ángulo alpha obtenido, debes girar el div (debe girar pues a la vez que giras tu móvil). Para ello no tienes más que usar las transformaciones mediante CSS (https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transforms/Using_CSS_transforms). La idea es pues cada vez que obtengo un nuevo ángulo (salta el evento) aplicar ese angulo mediante transformación al DIV: 
```js
document.getElementById("myDIV").style.transform = "rotate(7deg)";
``` 
Por tanto, es tan sólo cambiar el 7 del ejemplo anterior por el ángulo obtenido.

b) Una vez consigas rotar el DIV intenta aplicar transformaciones en 3D usando los 3 ángulos. Para ello puedes basarte en el siguiente tutorial: https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Using_device_orientation_with_3D_transforms

5) Cargar contenido dinámicamente usando AJAX. Crear una web en la que, mediante desplegables, pueda seleccionar una localidad. Inicialmente se cargan tan sólo las provincias. Al seleccionar una provincia, aparece otro desplegable con los municipios de esa provincia.

Estos datos (los listados de provincias iniciales, así como los listados de municipios para una provincia seleccionada) serán suministrados por una página en PHP que será llamada mediante AJAX. Dicha página deberá obtener esa información y enviarsela al usuario en un formato correcto de intercambio de datos (XML o JSON). Para obtener esos datos de municipios, en la web https://postal.cat/ los puedes encontrar en varios formatos (CSV, EXCEL o BD SQL), siendo decisión del alumno cual utilizar.

6. Añade las siguientes mejoras al ejercicio anterior :

◦ Permite que el usuario introduzca directamente un código postal, y en base a él se muestre el municipio o municipios a elegir.

7. Mejora el ejercicio anterior para hacer uso ahora de las predicciones meteorológicas que ofrece la AEMET, de tal modo que se muestre la predicción del tiempo para el municipio seleccionado. Actualmente se pueden consultar mediante XML las predicciones que genera la Agencia de Meteorología para cada municipio. Por tanto conociendo su código postal, podemos consultar los datos para un municipio. Toda la información la tienes en https://opendata.aemet.es/ (tienes hasta ejemplos de código).

Por tanto se pide:

• Añadir a tu web la posibilidad de consultar el tiempo para el municipio escogido. Para ello recuerda que al seleccionar un munipio ya dispones de su código postal, de modo que ahora desde tu PHP deberás consultar la URL correspondiente de la AEMET y enviar los datos al cliente (en el formato que tú decidas).

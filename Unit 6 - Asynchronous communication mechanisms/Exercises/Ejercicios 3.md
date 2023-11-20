# 1) Cargar contenido dinámicamente usando AJAX. Crear una web en la que, mediante desplegables, pueda seleccionar una comunidad. Inicialmente se cargan tan sólo las comunidades. Al seleccionar una, aparece otro desplegable con las provincias y así sucesivamente hasta llegar a los municipios de esa provincia.

Para obtener estos datos vamos a trabajar con una API que los proporciona: geoapi.es

Tu trabajo consiste en estudiar dicha API (cómo funciona, formatos de respuesta) y maquetar las respuestas recibidas. 

# 2) Mejora el ejercicio anterior para hacer uso ahora de las predicciones meteorológicas que ofrece la AEMET, de tal modo que se muestre la predicción del tiempo para el municipio seleccionado. Actualmente se pueden consultar mediante XML las predicciones que genera la Agencia de Meteorología para cada municipio. Por tanto conociendo su código postal, podemos consultar los datos para un municipio. Toda la información la tienes en https://opendata.aemet.es/ (tienes hasta ejemplos de código).

Por tanto se pide:

• Añadir a tu web la posibilidad de consultar el tiempo para el municipio escogido. Para ello recuerda que al seleccionar un munipio ya dispones de su código postal, de modo que ahora desde tu PHP deberás consultar la URL correspondiente de la AEMET y enviar los datos al cliente (en el formato que tú decidas).

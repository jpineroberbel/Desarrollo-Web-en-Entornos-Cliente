# 1) Cargar contenido dinámicamente usando AJAX. 
Crear una web en la que, mediante desplegables, pueda seleccionar una comunidad. Inicialmente se cargan tan sólo las comunidades. Al seleccionar una, aparece otro desplegable con las provincias y así sucesivamente hasta llegar a los municipios de esa provincia.

Para obtener estos datos vamos a trabajar con una API que los proporciona: geoapi.es

Tu trabajo consiste en estudiar dicha API (cómo funciona, formatos de respuesta) y maquetar las respuestas recibidas. 

# 2) Mejora el ejercicio anterior para hacer uso ahora de las predicciones meteorológicas que ofrece la AEMET, de tal modo que se muestre la predicción del tiempo para el municipio seleccionado. 

Actualmente se pueden consultar mediante JSON las predicciones por municipio. Toda la información la tienes en https://opendata.aemet.es/ (tienes hasta ejemplos de código).

Por tanto se pide añadir a tu web la posibilidad de consultar el tiempo para el municipio escogido. Para ello recuerda que al seleccionar un munipio ya dispones de su código de municipio


<img width="1024" height="1536" alt="interfaz" src="https://github.com/user-attachments/assets/97638c26-5b7a-4e91-bbc5-10a046fee91e" />

# Ejercicio: Maquetación de datos JSON con `<div>`

A continuación se proporciona un conjunto de datos en formato JSON que describe varios colores, junto con sus categorías, tipos y códigos en distintos formatos.

## Objetivo

Maquetar esta información utilizando únicamente elementos `<div>`, organizándola de forma clara y estructurada.

## Requisitos

- Crear un contenedor principal para todos los colores.
- Para cada color, generar un `<div>` individual que incluya:
  - Nombre del color
  - Categoría y tipo (si existe)
  - Código `rgba`
  - Código `hex`
- Cada `<div>` debe tener como color de fondo el color representado.
- Solo se permite usar elementos `<div>` para toda la estructura.

## Datos a maquetar

```json
{
  "colors": [
    {
      "color": "black",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,255,255,1],
        "hex": "#000"
      }
    },
    {
      "color": "white",
      "category": "value",
      "code": {
        "rgba": [0,0,0,1],
        "hex": "#FFF"
      }
    },
    {
      "color": "red",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,0,0,1],
        "hex": "#FF0"
      }
    },
    {
      "color": "blue",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [0,0,255,1],
        "hex": "#00F"
      }
    },
    {
      "color": "yellow",
      "category": "hue",
      "type": "primary",
      "code": {
        "rgba": [255,255,0,1],
        "hex": "#FF0"
      }
    },
    {
      "color": "green",
      "category": "hue",
      "type": "secondary",
      "code": {
        "rgba": [0,255,0,1],
        "hex": "#0F0"
      }
    }
  ]
}





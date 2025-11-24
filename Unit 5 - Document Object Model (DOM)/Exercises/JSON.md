
<img width="1024" height="1536" alt="interfaz" src="https://github.com/user-attachments/assets/97638c26-5b7a-4e91-bbc5-10a046fee91e" />

# Ejercicio 1: Maquetación de datos JSON con `<div>`

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
```

# Ejercicio 2: Maquetación de datos de Películas

A continuación se proporciona un conjunto de datos de películas en formato JSON.

## Objetivo

Maquetar esta información, organizándola de forma clara y estructurada.

```json
{
  "Search": [
    {
      "Title": "Star Wars: Episode IV - A New Hope",
      "Year": "1977",
      "imdbID": "tt0076759",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BOGUwMDk0Y2MtNjBlNi00NmRiLTk2MWYtMGMyMDlhYmI4ZDBjXkEyXkFqcGc@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode V - The Empire Strikes Back",
      "Year": "1980",
      "imdbID": "tt0080684",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BMTkxNGFlNDktZmJkNC00MDdhLTg0MTEtZjZiYWI3MGE5NWIwXkEyXkFqcGc@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode VI - Return of the Jedi",
      "Year": "1983",
      "imdbID": "tt0086190",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BNWEwOTI0MmUtMGNmNy00ODViLTlkZDQtZTg1YmQ3MDgyNTUzXkEyXkFqcGc@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode VII - The Force Awakens",
      "Year": "2015",
      "imdbID": "tt2488496",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BOTAzODEzNDAzMl5BMl5BanBnXkFtZTgwMDU1MTgzNzE@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode I - The Phantom Menace",
      "Year": "1999",
      "imdbID": "tt0120915",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BODVhNGIxOGItYWNlMi00YTA0LWI3NTctZmQxZGUwZDEyZWI4XkEyXkFqcGc@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode III - Revenge of the Sith",
      "Year": "2005",
      "imdbID": "tt0121766",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BNTc4MTc3NTQ5OF5BMl5BanBnXkFtZTcwOTg0NjI4NA@@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode II - Attack of the Clones",
      "Year": "2002",
      "imdbID": "tt0121765",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BNTgxMjY2YzUtZmVmNC00YjAwLWJlODMtNDBhNzllNzIzMjgxXkEyXkFqcGc@._V1_SX300.jpg"
    },
    {
      "Title": "Rogue One: A Star Wars Story",
      "Year": "2016",
      "imdbID": "tt3748528",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BMjEwMzMxODIzOV5BMl5BanBnXkFtZTgwNzg3OTAzMDI@._V1_SX300.jpg"
    },
    {
      "Title": "Star Wars: Episode VIII - The Last Jedi",
      "Year": "2017",
      "imdbID": "tt2527336",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BMjQ1MzcxNjg4N15BMl5BanBnXkFtZTgwNzgwMjY4MzI@._V1_SX300.jpg"
    },
    {
      "Title": "Star Trek",
      "Year": "2009",
      "imdbID": "tt0796366",
      "Type": "movie",
      "Poster": "https://m.media-amazon.com/images/M/MV5BMjE5NDQ5OTE4Ml5BMl5BanBnXkFtZTcwOTE3NDIzMw@@._V1_SX300.jpg"
    }
  ],
  "totalResults": "4947",
  "Response": "True"
}
´´´

# Ejercicio 3: Maquetación de datos de Películas II

Mejora el ejercicio anterior añadiendo un botón que cargue más películas. Al pulsarlo debes maquetar las siguientes:

´´´json
{"Search":[{"Title":"Star Wars: Episode IX - The Rise of Skywalker","Year":"2019","imdbID":"tt2527338","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BODg5ZTNmMTUtYThlNy00NjljLWE0MGUtYmQ1NDg4NWU5MjQ1XkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Trek Into Darkness","Year":"2013","imdbID":"tt1408101","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BMTk2NzczOTgxNF5BMl5BanBnXkFtZTcwODQ5ODczOQ@@._V1_SX300.jpg"},{"Title":"A Star Is Born","Year":"2018","imdbID":"tt1517451","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BNGUxZTc0NTAtNzQwMy00MmM2LTgzMGYtZWIyY2E1MGFjYmM5XkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Solo: A Star Wars Story","Year":"2018","imdbID":"tt3778644","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BOTM2NTI3NTc3Nl5BMl5BanBnXkFtZTgwNzM1OTQyNTM@._V1_SX300.jpg"},{"Title":"Star Trek Beyond","Year":"2016","imdbID":"tt2660888","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BN2FhNDI1YTYtNWI0OC00ZjYxLWJlYWEtN2ZiZjRmZDY1MWJjXkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Trek: The Next Generation","Year":"1987–1994","imdbID":"tt0092455","Type":"series","Poster":"https://m.media-amazon.com/images/M/MV5BMmNiNTQ2YzYtODBjYy00ZWMwLTlmNWMtYWE1NTQ2ZTYyZmMwXkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Trek: Discovery","Year":"2017–2024","imdbID":"tt5171438","Type":"series","Poster":"https://m.media-amazon.com/images/M/MV5BOTZkZTc1ZmYtYTA3Mi00MzZhLWFmZTItZTM2NThjYWJlZGU4XkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Wars: The Clone Wars","Year":"2008–2020","imdbID":"tt0458290","Type":"series","Poster":"https://m.media-amazon.com/images/M/MV5BOTdiODQ1MDYtZjM5My00MmQ5LTk1ZWUtZWIwYjBhZGMxZDAyXkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Trek: First Contact","Year":"1996","imdbID":"tt0117731","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BZjc0OWE1NDMtNjRmMi00ZDc2LWI2ZmQtNzEwNWU4Nzg4NDA5XkEyXkFqcGc@._V1_SX300.jpg"},{"Title":"Star Trek II: The Wrath of Khan","Year":"1982","imdbID":"tt0084726","Type":"movie","Poster":"https://m.media-amazon.com/images/M/MV5BOTFkZDY5NWQtMjY4Yy00OThiLTk3YjQtMDdhYTllMTI4MTdiXkEyXkFqcGc@._V1_SX300.jpg"}],"totalResults":"4947","Response":"True"};


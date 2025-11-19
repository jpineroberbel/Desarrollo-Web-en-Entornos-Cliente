# 🚀 Mini-Proyecto: Componentes para Página de Producto Interactiva

**Objetivo:** Construir la página de detalle de un producto para una tienda online. Este proyecto integra todos los conocimientos adquiridos: gestión de estado (`useState`), paso de información (`props`), renderizado condicional.


---

## 1. Objetivo Visual

El objetivo es crear una interfaz moderna igual a la siguiente:

(https://es.vecteezy.com/arte-vectorial/19533982-maquetas-de-pagina-de-interfaz-de-usuario-minimalista-moderna-para-comercio-electronico)

---

## 2. Datos Iniciales (Mock Data)

Copia y pega este objeto en tu archivo `App.js`. Simulará la base de datos del producto.

```javascript
const PRODUCT_DATA = {
  id: "p1",
  name: "Zapatillas Clásicas Runner",
  price: 120,
  variants: [
    {
      id: "v1",
      color: "Blanco",
      colorHex: "#FFFFFF",
      image: "[https://via.placeholder.com/400x400/f0f0f0/000000?text=Blanco](https://via.placeholder.com/400x400/f0f0f0/000000?text=Blanco)",
      stock: 10
    },
    {
      id: "v2",
      color: "Negro",
      colorHex: "#000000",
      image: "[https://via.placeholder.com/400x400/333333/ffffff?text=Negro](https://via.placeholder.com/400x400/333333/ffffff?text=Negro)",
      stock: 5
    },
    {
      id: "v3",
      color: "Rojo",
      colorHex: "#FF0000",
      image: "[https://via.placeholder.com/400x400/aa0000/ffffff?text=Rojo](https://via.placeholder.com/400x400/aa0000/ffffff?text=Rojo)",
      stock: 0 // ¡Sin stock!
    }
  ]
};

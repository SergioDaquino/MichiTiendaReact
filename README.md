MichiTienda - React (Vite) conversion
-------------------------------------

Esta es una conversión automática del proyecto original (HTML/CSS/JS) a una
aplicación React basada en Vite.

Requerimientos implementados (resumen):
- Carrito con useState y contexto (CartContext) + persistencia en localStorage.
- Listado de productos (Home) que consume https://fakestoreapi.com/products con manejo de carga y errores (useEffect).
- Páginas: Inicio (catalogo), Producto (ruta dinámica /producto/:id), Carrito, Nosotros.
- Rutas protegidas: /checkout solo accesible si el usuario está "logueado" (mock) — login via Navbar.
- Componentes reutilizables (ProductCard, Navbar, ProtectedRoute).
- Uso de useState, useEffect, react-router-dom.

Cómo usar:
1) En tu máquina, con Node.js instalado:
   npm install
   npm run dev

2) Abre http://localhost:5173

Notas:
- Se usan imágenes copiadas desde el proyecto original en public/img (si existían).
- La autenticación es simulada: presiona "Entrar" en la navbar para poder acceder a /checkout.
- Puedes cambiar la API en src/pages/Home.jsx y src/pages/ProductPage.jsx.


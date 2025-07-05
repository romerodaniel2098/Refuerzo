
#  Proyecto Bento Grid con HTML y CSS

Este proyecto recrea una **maqueta tipo Bento Grid**, estructurada visualmente con tarjetas (`cards`) organizadas mediante **CSS Grid y Flexbox**. El diseño está basado en una imagen de referencia y se adapta de forma responsiva a dispositivos móviles.

---

##  Estructura del proyecto

```
proyecto-bento/
├── index.html
├── style.css
└── assets/
    └── images/
        ├── illustration-create-post.webp
        ├── illustration-ai-content.webp
        ├── illustration-five-stars.webp
        ├── illustration-audience-growth.webp
        ├── illustration-grow-followers.webp
        └── illustration-consistent-schedule.webp
```

---

##  Descripción del código

### `index.html`

El HTML está compuesto por un `<main>` con la clase `grid-container` que contiene dos secciones principales:

- **`.column-1`**: columna izquierda (1/4 del ancho), contiene tarjetas verticales (`.tall`) y normales.
- **`.column-2`**: columna derecha (3/4 del ancho), es una **subgrid de 3x3** donde se distribuyen el resto de las tarjetas.

Cada tarjeta (`.card`) puede tener modificadores:
- `.wide` → ocupa 2 columnas.
- `.tall` → ocupa 2 filas.
- Colores: `.purple`, `.beige`, `.orange`, `.yellow`, `.white`, `.light-purple`.

Ejemplo:

```html
<div class="card purple wide">
  <img src="..." alt="..." />
  <h3>Grow followers with non-stop content.</h3>
</div>
```

---

### `style.css`

El CSS incluye:

- **Reset básico** con `box-sizing: border-box`.
- Grid principal (`.grid-container`) con 4 columnas.
- Subgrid interna en `.column-2` de 3 columnas y 3 filas.
- Tarjetas con **bordes redondeados**, sombras, y colores personalizados.
- Modificadores de tamaño: `.wide`, `.tall`.
- Estilos responsivos (`@media`) para dispositivos menores a 768px.

---

##  Responsividad

En pantallas pequeñas:
- La grilla se convierte en una sola columna.
- Las tarjetas se adaptan automáticamente.
- Las tarjetas `.wide` y `.tall` se vuelven normales.

---

##  Requisitos para que funcione

1. Mantener la estructura de carpetas.
2. Las imágenes deben estar en `assets/images/`.
3. Asegúrate de que `style.css` esté vinculado correctamente en el `<head>` del HTML.

---

##  Personalización

Puedes modificar:
- Colores de fondo en el CSS (`.purple`, `.yellow`, etc.).
- Distribución de tarjetas (cambiando o combinando `.wide` y `.tall`).
- Imágenes, texto o efectos hover según necesites.


---

##  Autor

Daniel Romero García  
Proyecto educativo/práctico  

# La importancia del formato físico en las consolas

## Propósito de la página

Página informativa que explica por qué el formato físico de los
videojuegos (cartuchos, discos y sus cajas) sigue siendo relevante
frente al auge del formato digital. Está dirigida a jugadores,
coleccionistas y cualquier persona interesada en la conservación de
videojuegos, cerrando con una conclusión que invita a valorar las
ventajas de cada formato.

## Estructura del proyecto

```
formato-fisico-consolas/
├── index.html
├── styles.css
├── assets/
│   └── caja-videojuego.svg
└── README.md
```

## Cómo visualizar la página

1. Descarga o clona esta carpeta completa (debe mantenerse la
   estructura de archivos, ya que `index.html` referencia `styles.css`
   y `assets/caja-videojuego.svg` con rutas relativas).
2. Abre `index.html` directamente en cualquier navegador.
3. Alternativamente, si el proyecto está en GitHub Pages, visita el
   enlace publicado (agregar aquí el enlace una vez publicado).

## Semántica HTML5 aplicada

- `<header>` agrupa el logo del sitio y la navegación principal.
- `<nav>` con `aria-label="Navegación principal"` identifica los
  enlaces internos a cada sección.
- `<main>` contiene el único bloque de contenido central de la página.
- `<section>` divide el contenido en bloques temáticos: introducción,
  ventajas del formato físico, riesgos del formato digital y
  conclusión, cada uno vinculado a su encabezado mediante
  `aria-labelledby`.
- `<article>` se usa para cada ventaja del formato físico, ya que
  representa contenido autocontenido y reutilizable.
- `<aside>` anidado dentro de la sección de riesgos incluye un dato
  relacionado sobre el cierre real de la PlayStation Store para PS3 y
  PS Vita anunciado por Sony en 2026, secundario respecto al
  contenido principal de esa sección.
- `<footer>` cierra la página con información de autoría.
- Jerarquía de encabezados respetada: un solo `<h1>` (título
  principal), `<h2>` por sección y `<h3>` dentro de tarjetas/artículos.

## Accesibilidad aplicada

- **Enlace de salto** (`skip-link`) que permite a los usuarios de
  teclado saltar directamente al contenido principal.
- **Foco visible** en todos los elementos interactivos mediante
  `:focus-visible`, para una navegación con teclado (Tab) clara.
- **Imagen con `alt` descriptivo**: la ilustración de la caja de
  videojuego incluye un texto alternativo que la describe para
  lectores de pantalla.
- **Atributos ARIA**: `aria-labelledby` conecta cada sección (y el
  `<aside>` de dato relacionado) con su encabezado correspondiente.
- **Contraste de color**: texto oscuro (#1c1c1c) sobre fondo claro
  (#faf7f2), y header/footer en blanco sobre azul petróleo oscuro
  (#0f4c5c), cumpliendo un contraste adecuado (nivel AA).
- **Idioma declarado**: `<html lang="es">` para la correcta
  pronunciación en lectores de pantalla.

## Validación

El archivo `index.html` fue verificado con el
[W3C Markup Validation Service](https://validator.w3.org/) para
confirmar que no contiene errores de sintaxis.

## Recursos

- `assets/caja-videojuego.svg`: ilustración vectorial creada
  específicamente para este ejercicio, sin restricciones de derechos
  de autor.

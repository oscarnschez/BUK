# BÜK.

**READ. THINK. REBEL.**
*A digital library of ideas. An archive of radical reading.*

BÜK. es un archivo personal para registrar los libros físicos que compras: cada libro recibe un número de inventario y una sección numerada, y puedes buscarlo por título, autor, categoría o ISBN.

## Funciones

- **Inicio:** cifras del archivo, un libro del archivo cada día, buscador y secciones numeradas.
- **Archivo:** cuadrícula de inventario (`001 / FILOSOFÍA`) o vista de lomos en estantería.
- **Ficha:** portada, sinopsis, datos bibliográficos, estado de lectura, calificación y préstamos. El botón de recurso digital solo aparece si guardaste un enlace.
- **Panel de control:** todos los registros en una hoja tipo Excel, con fecha y hora de registro, edición en celda y exportación a `.xlsx`.
- **Informe:** plan de lectura del año, libros por sección, distinciones y un cartel descargable.
- **Identidad:** logotipo en sus variantes (horizontal, compacta, monocromática, favicon e ícono de app), paleta y tipografía.
- Funciona sin conexión una vez visitada y se puede instalar en el teléfono.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub, por ejemplo `buk`.
2. Sube **el contenido** de esta carpeta a la raíz del repositorio (`index.html` debe quedar en la raíz, no dentro de otra carpeta). Desde la web: *Add file → Upload files* y arrastra todos los archivos y la carpeta `icons`.
3. En el repositorio: *Settings → Pages → Build and deployment*. En *Source* elige **Deploy from a branch**, rama **main**, carpeta **/ (root)**, y guarda.
4. En uno o dos minutos la app estará en `https://TU-USUARIO.github.io/buk/`.

## Instalar en el teléfono

- **iPhone (Safari):** abre la dirección, toca *Compartir* y luego *Agregar a inicio*.
- **Android (Chrome):** abre la dirección y toca *Instalar app* en el menú.

## Dónde se guardan tus libros

En esta versión los libros se guardan **en el navegador** de cada dispositivo (`localStorage`):

- Lo que registres en el teléfono no aparece en la computadora, y al revés.
- Si borras los datos del sitio en el navegador, se borra el archivo. Exporta a Excel de vez en cuando como respaldo.
- No se sincroniza con la versión de BÜK. publicada en Claude, que guarda los libros en tu cuenta de Claude.

El **Bibliotecario** (recomendaciones según tu ánimo) solo existe en la versión de Claude, porque usa a Claude para elegir.

## Archivos

```
index.html              La app completa (HTML, CSS y JavaScript en un solo archivo)
manifest.webmanifest    Datos para instalarla como app
sw.js                   Service worker: funcionamiento sin conexión
icons/                  Favicon e íconos de la app
```

## Créditos

- Tipografías: [Archivo](https://fonts.google.com/specimen/Archivo) e [IBM Plex Sans Condensed](https://fonts.google.com/specimen/IBM+Plex+Sans+Condensed), licencia SIL Open Font, servidas por Google Fonts.
- Exportación a Excel: [SheetJS](https://sheetjs.com), cargada desde cdnjs solo al exportar.

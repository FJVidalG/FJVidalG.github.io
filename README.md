# Portfolio · Francisco Jesús Vidal García

Portfolio personal publicado con GitHub Pages: **https://fjvidalg.github.io**

Página única, sin dependencias ni proceso de compilación. Todo el CSS y las imágenes van embebidos en `index.html`, de modo que solo carga un recurso externo —las tipografías de Google Fonts— y funciona igual dentro de diez años.

## Contenido

| Archivo | Qué es |
|---------|--------|
| `index.html` | La página completa: estructura, estilos, capturas e ilustraciones |
| `CV_Francisco_Vidal.pdf` | Currículum enlazado desde la página |
| `.nojekyll` | Desactiva el procesado Jekyll de GitHub Pages: el sitio se sirve tal cual |

## Detalles técnicos

Las capturas de pantalla y el diagrama del modelo de datos están embebidos como **data URI en WebP**, unos 100 KB en total. Evita peticiones adicionales y garantiza que la página no se rompa si algún archivo se mueve de sitio.

El diagrama entidad-relación es **SVG escrito a mano**, no una imagen exportada. Pesa 5 KB, es texto seleccionable, escala sin pixelarse y toma sus colores de las variables CSS, así que se adapta solo al tema claro y al oscuro.

El tema sigue la preferencia del sistema mediante `prefers-color-scheme`, con la paleta completa definida en `:root` y redefinida para modo oscuro. La maquetación usa CSS Grid y baja a una columna por debajo de 760 px.

## Publicar cambios

```bash
git add index.html
git commit -m "Actualiza el portfolio"
git push
```

GitHub Pages reconstruye el sitio en menos de un minuto.

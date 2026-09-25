# Portfolio · Francisco Jesús Vidal García

Portfolio personal publicado con GitHub Pages: **https://fjvidalg.github.io**

Página estática escrita a mano, sin frameworks ni proceso de compilación. El único recurso externo son las tipografías de Google Fonts.

## Contenido

| Archivo | Qué es |
|---------|--------|
| `index.html` | La página completa: estructura, estilos y diagramas |
| `img/` | Capturas de pantalla de los proyectos, en WebP |
| `CV_Francisco_Vidal.pdf` | Currículum enlazado desde la página |
| `.nojekyll` | Desactiva el procesado Jekyll de GitHub Pages: el sitio se sirve tal cual |

## Detalles técnicos

Los diagramas (el modelo de datos de PsyTrack y los dos de flujo) son **SVG escritos a mano** dentro del HTML, no imágenes exportadas. Pesan unos pocos kilobytes, el texto es seleccionable, escalan sin pixelarse y toman sus colores de las variables CSS, así que se adaptan solos al tema claro y al oscuro.

Las capturas están en **WebP**, con carga diferida (`loading="lazy"`) y dimensiones declaradas en el HTML para que la página no salte mientras se cargan.

El tema sigue la preferencia del sistema mediante `prefers-color-scheme`, con la paleta definida en `:root` y redefinida para modo oscuro. La maquetación usa CSS Grid y pasa a una columna por debajo de 760 px.

## Publicar cambios

```bash
git add .
git commit -m "Actualiza el portfolio"
git push
```

GitHub Pages reconstruye el sitio en menos de un minuto.

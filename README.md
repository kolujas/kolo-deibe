# Kolo Deibe

Sitio para publicar mis escritos: textos oscuros, viscerales, cargados de introspección.

Todo vive en un solo archivo, [index.html](index.html), sin dependencias ni build.

## Qué tiene

- Portada con luna, niebla y reflejo en el agua, dibujada en canvas.
- Índice de escritos, del más reciente al más antiguo, con filtro por etiqueta.
- Lectura a pantalla completa con fecha, palabras y minutos de lectura; cada escrito tiene su link (`#id`).
- Dos formas de texto: **prosa** (párrafos con sangría y letra capital) y **verso** (respeta los saltos de línea).
- Editor con borrador local, etiquetas e imagen de portada opcional.

## Dónde se guardan los escritos

Hoy la página corre como Artifact de claude.ai y guarda los escritos y la portada en su base de datos
(`window.claude.use("db")`), y las imágenes en su almacén de archivos (`use("assets")`).
Solo el dueño puede publicar; el resto lee.

Si se abre `index.html` fuera de claude.ai, la página se ve igual pero no tiene de dónde leer escritos
ni dónde guardarlos. Para publicarla por su cuenta (por ejemplo en GitHub Pages) hace falta cambiar esa
capa por otro backend.

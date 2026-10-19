# Kolo Deibe

Sitio para publicar mis escritos: textos oscuros, viscerales, cargados de introspección.

Se publica en **https://kolujas.github.io/kolo-deibe/** con GitHub Pages. No tiene build ni dependencias.

## Qué tiene

- Portada con luna, niebla y reflejo en el agua, dibujada en canvas.
- Índice de escritos, del más reciente al más antiguo, con filtro por etiqueta.
- Lectura a pantalla completa con fecha, palabras y minutos de lectura; cada escrito tiene su link (`#id`).
- Dos formas de texto: **prosa** (párrafos con sangría y letra capital) y **verso** (respeta los saltos de línea).
- Editor con borrador local, etiquetas e imagen de portada opcional.

## Dónde está cada cosa

| Archivo | Qué guarda |
| --- | --- |
| `index.html` | La página entera: estilos, lectura y editor. |
| `datos/escritos.json` | Todos los escritos. |
| `datos/sitio.json` | Nombre, presentación e Instagram de la portada. |
| `imagenes/` | Las imágenes de portada, achicadas a 1600 px. |

## Cómo se publica

Cualquiera puede leer. Para escribir se entra a **https://kolujas.github.io/kolo-deibe/#autor**
(la página no tiene link a esa pantalla) y se pega una clave de
GitHub (fine-grained token) con permiso **Contents: Read and write** solo sobre este repo. La clave queda
guardada en ese navegador y nada más.

Cada vez que publicás, editás o borrás, la página hace un commit en `main` con la API de GitHub, y
GitHub Pages lo muestra a los lectores en alrededor de un minuto. También se puede editar a mano
`datos/escritos.json` y hacer push.

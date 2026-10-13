# Cuánto sabes del Tricanter

Cuestionario web estático con 20 preguntas e imágenes, alternativas aleatorias, corrección inmediata, explicación, puntaje final y descarga del resultado individual en CSV.

## Publicar en GitHub Pages

1. Descomprime el ZIP en tu computador.
2. Crea un repositorio público en GitHub, por ejemplo cuestionario-tricanter.
3. En Add file > Upload files, sube index.html, questions.json, README.md y la carpeta assets completa. Conserva la carpeta assets y sus imágenes. index.html debe quedar en la raíz del repositorio, no dentro de otra carpeta. Sube los archivos descomprimidos, no el ZIP.
4. Confirma la subida con Commit changes.
5. Ve a Settings > Pages. En Source selecciona Deploy from a branch. Selecciona la rama main y la carpeta /(root), luego Save.
6. Espera a que termine la publicación. GitHub mostrará el enlace en Pages.

Documentación oficial: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Probar en tu computador

No abras index.html con doble clic: las preguntas se cargan desde un archivo JSON y necesitan un servidor web. Si tienes Python instalado, abre una terminal en esta carpeta y ejecuta:

python -m http.server 8000

Después abre http://localhost:8000.

## Funcionamiento

Cada primera elección queda registrada. La corrección aparece de inmediato; puedes volver a preguntas anteriores para revisar, y descargar un CSV al finalizar. Los nombres y resultados se mantienen en la sesión del navegador y no se envían a una base de datos. No requiere API de inteligencia artificial ni claves.

## Fuente de contenido

Imágenes y contenidos técnicos del folleto Flottweg sobre centrífugas para aceite de oliva, edición 06/2013, facilitado para este proyecto. El cuestionario evalúa principios de separación y reconocimiento de componentes. Su uso operativo minero requiere adecuación al equipo y a los procedimientos de la faena.

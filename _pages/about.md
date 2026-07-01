---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Esta es la página principal de un sitio web que utiliza la plantilla [Academic Pages](https://github.com/academicpages/academicpages.github.io) y está alojado en GitHub Pages. [GitHub Pages](https://pages.github.com) es un servicio gratuito que permite crear y alojar sitios web a partir del código y los datos almacenados en un repositorio de GitHub, actualizándose automáticamente con cada nueva confirmación. Esta plantilla se derivó del tema [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), creado por Michael Rose, y se amplió para admitir el tipo de contenido que suelen tener los académicos: publicaciones, charlas, docencia, portafolio, entradas de blog y un currículum vitae generado dinámicamente. Además, estas mismas características la convierten en una excelente plantilla para cualquiera que necesite una imagen profesional.

Puedes bifurcar [esta plantilla](https://github.com/academicpages/academicpages.github.io) ahora mismo, modificar la configuración y los archivos Markdown, añadir tus propios PDF y otro contenido, ¡y tener tu propio sitio web gratis y sin anuncios!

Un sitio web personal basado en datos
======
Al igual que muchas otras plantillas de GitHub Pages basadas en Jekyll, Academic Pages te obliga a separar el contenido del diseño del sitio web. El contenido y los metadatos de tu sitio web se encuentran en archivos Markdown estructurados, mientras que otros archivos conforman el tema, especificando cómo transformar ese contenido y metadatos en páginas HTML. Guardas estos archivos Markdown (.md), YAML (.yml), HTML y CSS en un repositorio público de GitHub. Cada vez que confirmas y subes una actualización al repositorio, el servicio [GitHub Pages](https://pages.github.com/) crea páginas HTML estáticas basadas en estos archivos, que se alojan gratuitamente en los servidores de GitHub.

Muchas de las funcionalidades de los sistemas de gestión de contenido dinámico (como WordPress) se pueden lograr de esta manera, utilizando una fracción de los recursos computacionales y con mucha menos vulnerabilidad a ataques informáticos y DDoS. También puedes modificar el tema a tu gusto sin tocar el contenido de tu sitio. Si llegas a un punto en el que has dañado irreparablemente algo en Jekyll/HTML/CSS, tus archivos Markdown que describen tus charlas, publicaciones, etc., estarán a salvo. Puedes revertir los cambios o incluso eliminar el repositorio y empezar de nuevo; ¡solo asegúrate de guardar los archivos Markdown! También puedes escribir scripts que procesen los datos estructurados del sitio, como [este](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) que analiza los metadatos de las páginas sobre charlas para mostrar [un mapa de todas las ubicaciones donde has dado una charla](https://academicpages.github.io/talkmap.html).

Para aquellos usuarios que necesiten funcionalidades más avanzadas, la plantilla también es compatible con las siguientes herramientas populares:
- [MathJax](https://www.mathjax.org/) para ecuaciones matemáticas
- [Mermaid](https://mermaid.js.org/) para diagramas
- [Plotly](https://plotly.com/javascript/) para gráficos

Primeros pasos
======
1. Crea una cuenta de GitHub si no tienes una y confirma tu correo electrónico (¡obligatorio!).
2. Crea un fork de [esta plantilla](https://github.com/academicpages/academicpages.github.io) haciendo clic en el botón "Usar esta plantilla" en la esquina superior derecha.

3. Ve a la configuración del repositorio (el elemento de la derecha en las pestañas que comienzan con "Código" debería estar debajo de "Dejar de seguir"). Cambia el nombre del repositorio a "[tu nombre de usuario de GitHub].github.io", que también será la URL de tu sitio web.
1. Configure la configuración general del sitio y cree el contenido y los metadatos (vea a continuación; consulte también [este conjunto de diferencias](https://archive.is/3TPas) que muestra los archivos que se modificaron para configurar [un sitio de ejemplo](https://getorg-testacct.github.io) para un usuario con el nombre de usuario "getorg-testacct").
1. Suba cualquier archivo (como PDF, archivos .zip, etc.) al directorio `files/`. Aparecerán en https://[su nombre de usuario de GitHub].github.io/files/example.pdf.

1. Compruebe el estado accediendo a la configuración del repositorio, en la sección "Páginas de GitHub".

Configuración general del sitio
------
El archivo de configuración principal del sitio se encuentra en el directorio base, en [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), que define el contenido de las barras laterales y otras funciones generales del sitio. Deberás reemplazar las variables predeterminadas con información sobre ti y el repositorio de GitHub de tu sitio. El archivo de configuración del menú superior se encuentra en [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). Por ejemplo, si no tienes un portafolio ni entradas de blog, puedes eliminar esos elementos del archivo navigation.yml para que no aparezcan en el encabezado.

Crear contenido y metadatos
------ 
Para el contenido del sitio, hay un archivo Markdown para cada tipo de contenido, que se almacenan en directorios como _publications, _talks, _posts, _teaching o _pages. Por ejemplo, cada charla es un archivo Markdown en el directorio [_talks](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). Al principio de cada archivo Markdown hay datos estructurados en YAML sobre la charla, que el tema mostrará.

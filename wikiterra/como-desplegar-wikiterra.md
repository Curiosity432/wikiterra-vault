---
dg-home: false
dg-publish: true
---

> WikiTerra usa de base en local la app [Obsidian.md](https://obsidian.md/) y está construida gracias al plugin [Obsidian Digital Garden](https://github.com/oleeskild/obsidian-digital-garden) con el tema "Primary", usando GitHub para almacenar el contenido y Vercel para desplegarlo. Todo los artículos son notas escritas en formato markdown con enlaces a imágenes u otros contenidos.

## Formas de crear un página web

El estándar de internet y de los navegadores web es leer archivos [HTML](https://en.wikipedia.org/wiki/HTML), [CSS](https://en.wikipedia.org/wiki/CSS) y [JS](https://en.wikipedia.org/wiki/HTML), no hay nada que se salga de ahí.

La forma tradicional de crear páginas webs era escribir en formato HTML para crear la estructura, mediante CSS darle forma y con JS hacer animaciones, validaciones, contadores, etc. en la parte visual. Luego para la parte trasera la se creaba una base de datos relacional que procesase la información, usando PHP o cualquier otro lenguaje que se almacene los datos en lenguaje SQL, de esta forma la computadora que sirve los datos (servidor web) también almacenaba un registro.

Para hacer lo anterior se requiere de bastantes conocimientos, sin embargo hoy en día existen otras formas más sencillas de crear páginas web.

Si queremos hacer una página web que muestre información y que no la procese lo mejor es no usar una base de datos, y meter todo la información en archivos HTML. Y usar CSS y JS para hacer visualmente más atractivo.

Sin embargo conocer HTML, CSS, JS sigue siendo algo complicado por eso han surgido el uso de lenguajes de marcas más sencillos como [MarkDown (MD)](https://en.wikipedia.org/wiki/Markdown). Con un lenguaje más sencillo ahora solo necesitamos de una aplicación que nos convierta el contenido a formato web (HTML, CSS).

Lo bueno de MarkDown es que se puede entender fácilmente en texto plano y con aplicaciones podemos convertirlo o compilarlo en HTML y personalizarlo mediante el uso de temas ya creados con CSS.

Según el uso que le vayamos a dar las aplicaciones las podemos usar en local o servir para que la gente lo vea a través de internet.

## Gestores de notas o wikis personales para [PKM](https://en.wikipedia.org/wiki/Personal_knowledge_management)
- [Dendron.so](https://www.dendron.so/). Gestor de notas que funciona como una extensión de VSCode, soporta etiquetado, enlaces, búsquedas, visor de grafos. Similar a Obsidian.md.
- [Notion.so](https://www.notion.so/). Gestor de notas online (en markdown) colaborativo para crear documentación, wikis o gestionar proyectos.
- [Zim Wiki](https://zim-wiki.org/). Gestor de notas enfocado a crear wikis, más sencillo que Obsidian.md.
- [Obsidian.md](https://obsidian.md/). Gestor de notas (markdown) en local con visor de grafos, enlaces, búsquedas y multitud de plugins (extensiones).
	- Plugins para Obsian.md
		- [Obsidian Digital Garden](https://github.com/oleeskild/obsidian-digital-garden)
			- Pros. Configuración sencilla y despliegue gratuito.
			- Contras. Hay que usar dos plataformas, una para almacenar el contenido (GitHub) y otra para mostrarlo (Vercel o Netlfy).
		- [Perlite](https://github.com/secure-77/Perlite). 
			- Pros. Replica visual de Obsidian.md en la web.
			- Contras. Hay que configurar un servidor (Ngnx o Apache) y mantenerlo cuesta un mínimo 2€/mes.

## Generador de sitios estáticos ([SSG](https://en.wikipedia.org/wiki/Static_site_generator))

> Todos usan Markdown.
- [HUGO framework](https://gohugo.io/).
	- Pros.
		- [Se puede combinar con el uso de imágenes con Obsidian.md](https://discourse.gohugo.io/t/help-with-link-images-to-see-from-absolute-path-including-static/41177/3).
		- Multitud de plantillas a elegir (gratis y de pago)
		- Contras.
			- Crear temas requiere de HTML, CS y JS
			- Hay que servir el contenido en local para visualizarlo.
- [Docsify.js](https://docsify.js.org/#/)
	- Pros. 
		- Fácil configuración.
		- Funciona con formato markdown
	- Contras. 
		- Requiere de JavaScript en el navegador.
		- No hay jerarquía de carpetas con subcarpetas.
		- La barra lateral o índice hay que crearla enlazando todos los artículos en `_sidebar.md`.
- [Docusaurius.io](https://docusaurus.io/).
	- Contras.
		- Configuración enrevesada.
		- Precisa de muchos archivos
- [mdBook](https://github.com/rust-lang/mdBook).
	- Pros. 
		- Configuración sencilla.
		- Programado en Rust.
		- Modo de búsqueda integrado.
	- Contras. 
		- Orientado para libros o documentación con pasos.
		- Necesario crear enlaces en `summary.md`.
- [MKDocs](https://www.mkdocs.org/), [MKDocs material](https://github.com/squidfunk/mkdocs-material)
	- Pros. 
		- Buscador integrado.
		- Permite organizar artículos en árbol jerárquico.
	- Contras.
		- Configuración enrevesada.
		- La barra lateral o índice hay que crearla enlazando todos los artículos en `mkdocs.yml`.
- [NextBook](https://next-book.vercel.app/intro). 
	- Pros.
		- Configuración sencilla.
		- Permite enlazar imágenes.
	- Contras.
		- No hay buscador.
		- No hay jerarquía de carpetas con subcarpetas.
		- La barra lateral o índice hay que crearla enlazando todos los artículos en `config.json`.
- [Retype](https://retype.com/). 
	- Pros. 
		- Configuración sencilla.
		- Buscador integrado.
	- Contras. 
		- No hay jerarquía de carpetas con subcarpetas.
		- La barra lateral o índice hay que crearla enlazando todos los artículos en `retype.yml`.
- [Vuepress - VueJS](https://vuepress.vuejs.org/)
	- Pros.
		- Renderiza HTML.
		- Framework consolidado de JavaScript
	- Contras.
		- Requiere saber Typescript
		- Instalación con yarn


## Otras aplicaciones para generar contenido
### Gestores de contenido ([CMS](https://en.wikipedia.org/wiki/Content_management_system))
- Con base de datos relacional y lenguaje PHP en el lado servidor.
	- [WordPress](https://wordpress.org/). El CMS más usado del mundo con unos 810 millones de webs 43% del total de sitios webs, cuenta con multitud de extensiones y una gran comunidad.
	- [Drupal](https://www.drupal.org/). CMS similar a WordPress pero más simple.
	- [Joomla](https://www.joomla.org/). Otro CMS similar a los anteriores.
- Sin base de datos (Flat-CMS):
	-  [Grav](https://getgrav.org/). CMS que no requiere de base de datos, permite instalar plugins y se escribe en markdown. Además tiene en mente el uso de un instalador de paquetes. 

### Software de WIkis
- [DokuWiki](https://dokuwiki.org/). Software para crear wikis que no requiere base de datos, fácil de usar y con compatibilidad con markdown.
- [MediaWiki](https://www.mediawiki.org/wiki/Download), motor de la página Wikipedia desarrollado por Wikimedia (fundación de Wikipedia). Requiere de una base de datos relacional.
- [TiddleWiki](https://tiddlywiki.com/), es una wiki personal en un solo archivo HTML, sin base de datos, permite organizar información en notas y tener una sección de ellas. Para guardar el contenido hay que generar un nuevo archivo pulsando el botón "Save Wiki".
- [FeatherWiki](https://feather.wiki/), es una versión de pluma ("feather") de TiddlyWiki mucho más liviana.
- [Wiki.js](https://js.wiki/), el contenido es guardado en archivos markdown y cuenta con un panel de administración. Usa node.js entorno que se ejecuta en el lado servidor y requiere de una base de datos

> Nota: todas las aplicaciones citadas, excepto Obsidian.md y Notion son de software libre. Sin embargo los plugins de Obsidian.md sí son de código abierto y el cliente JS de notion también.


## Desplegar y hospedar webs

### Despliegue de sitios web estáticos
La mayoría de páginas webs hay que pagar por el servidor, sin embargo las webs que no precisan de base de datos se pueden desplegar de forma gratuita en la siguientes plataformas, con un dominio predeterminado.
- [Cloudfare Pages](https://pages.cloudflare.com/)
- [Codeberg Pages](https://codeberg.page/)
- [Deply HQ](https://www.deployhq.com/)
- [Fly.io](https://fly.io/)
- [GitHub Pages](https://pages.github.com/)
- [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/)
- [harp JS](https://harpjs.com/)
- [Netlify](https://app.netlify.com/signup)
- [Surge](https://surge.sh/)
- [TIiny](https://tiiny.host/)

## Referencias

<iframe style="border: 0; width: 100%; height: 450px;" allowfullscreen frameborder="0" src="https://raindrop.io/Interneto/documentation-app-28730066/embed/theme=dark&sort=title"></iframe>

<iframe style="border: 0; width: 100%; height: 450px;" allowfullscreen frameborder="0" src="https://raindrop.io/Interneto/documentation-wikis-28899661/embed/sort=title&theme=dark"></iframe>

<iframe style="border: 0; width: 100%; height: 450px;" allowfullscreen frameborder="0" src="https://raindrop.io/Interneto/ssg-deploy-20160335/embed/theme=dark"></iframe>

- [Documentation apps - Interneto](https://raindrop.io/Interneto/documentation-app-28730066)
- [Documentation wikis - Interneto](https://raindrop.io/Interneto/documentation-wikis-28899661)
- [SSG Deploy - Interneto](https://raindrop.io/Interneto/ssg-deploy-20160335/)
- [List of wiki software - Wikipedia](https://en.wikipedia.org/wiki/List_of_wiki_software)

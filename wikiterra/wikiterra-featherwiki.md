---
dg-home: false
dg-publish: true
---

# ¿Qué es WikiTerra-FeatherWiki?

- Archivos en la nube:
	- [WikiTerra FeatherWiki · Codeberg](https://codeberg.org/curiosity432/wikiterra-featherwiki)
	 - [WikiTerra FeatherWiki · GitHub](https://github.com/Curiosity432/wikiterra-featherwiki)

## ¿Qué es WikiTerra-FeatherWiki?
WikiTerra-FeatherWiki es una pequeña enciclopedia de la Tierra en pruebas gestionada entera sobre un HTML editable.

## FeatherWiki
Es una versión ligera de [TiddlyWiki](https://tiddlywiki.com/) el software que permite crear wikis, ya sea blog de notas, información personal, etc. TiddlyWiki tiene muchas características pero la más destacable es poder organizar toda la información en un solo archivo HTML editable, que permite añadir imágenes, temas personalizados, cifrado con contraseña... Además ocupa muy poco espacio en memoria y como cualquier elemento de desarrllo se puede sincronizar usando Git con un repositorio online como GitLab, GitHub, Gitea o un servidor propio.

## Ver contenido
Para ver el contenido lo único que hay que hacer es descargar el HTML desde el link en crudo [wikiterra-featherwiki.html](https://raw.githubusercontent.com/Curiosity432/WikiTerra-TiddlyWiki/main/WikiTerra.html) o desde el repositorio de [WikiTerra FeatherWiki de GitHub](https://github.com/Curiosity432/wikiterra-featherwiki).

Para abrirlo solo hace falta un navegador web como (Chrome, Firefox, MS Edge, etc). Una vez abierto ya podremos ver y editar en local.

## Editar
Si quieres editar puedes hacerlo en local, pero para que estos se cambien se apliquen en el repositorio de WikiTerra es necesario hacer un "fork" una copia en una nueva rama de GItHub y luego realizar una "Pull request".

Hay dos formas de hacerlo:
1. Usar solo GItHub, fork desde GItHub, editar en GitHub Codespaces y hacer "pull request".
2. Hacer un fork, editar en local con un IDE como VSCode, subir los cambios con git (con GUI o CLI) y  hacer "pull request". Para este método hay que conocer como funciona "git" desde la terminal (CLI) o usar una interfaz gráfica (GUI).

### Normas de edición
Hacer una enciclopedia no es una tarea sencilla, en este caso WikiTerra es una Beta en pruebas con el objetivo de ser un enciclopedia seria accesible para todo el mundo.
1. La información ha de ser objetiva, hay que intentar dejar de lado los aspectos subjetivos y escribir usando evidencias que sean comprobables y empíricas.
2. Esciribir con adecuación al tema y sentido.
3. No cometer errores ortgráficos, ni gramáticos.
4. Usar un tiempo verbal estándar (presente a ser posible).
5. No escribir opiniones personales, si se trata de una opinión ha de llevar argumentos verificables.
6. Intentar poner referencias de los hechos para verificar la autenticidad de los hechos.

---

## Pros vs contras de FeatherWiki
- **Ventajas (pros)**
	- Toda la inforamción está contenida en un archivo.
	- Se puede ver tanto online como en local.
	- En caso de pérdida si se mantiene el archivo la enciclopedia permanece.
- **Desventajas (contras)**
	- Para editar la información es necesario un navegador y usar html o markdown.
	- Para subir el cotenido a GItHub hay que saber usar Git.
# Web del Grupo de Usuarios de R Almería

Este es el repositorio de la página web del Grupo de Usuarios de R Almería, creada mediante [Jekyll][1], [Markdown][2] y `HTML/CSS`.

**Web en proceso de cambios de diseño y contenido**.

### ¿Cómo está construida?

La maquetación principal está hecha con`HTML/CSS`, sin embargo cada página individual está escrita en `markdown` con la idea de simplificar su creación y mantener un estilo uniforme.

Para las tareas de construcción, el encargado será **[Jekyll][1]**.

La web está basada en la página de [Hacklab Almería](http://www.hacklabalmeria.net).

### ¿Cómo instalar Jekyll?

#### GNU/Linux

En distribuciones basadas en _Debian_ bastará un `apt-get install jekyll`. Como norma general, siempre se puede instalar usando las _gems_ de _Ruby_, `gem install jekyll`.

#### Windows

Para instalar [Jekyll][1] en el sistema de Microsoft puedes seguir [este tutorial][3].

#### Mac OS X

Puede instalarse usando las _gems_ de _ruby_, `gem install jekyll`. Requiere las [Command Line Tools de XCode][4].

### ¿Cómo usar Jekyll?

Bastará con ir a la carpeta raíz de la web y ejecutar `jekyll serve`. Ésto levantará un servidor local en la url por defecto `localhost:4000`, que nos permitirá visualizar los cambios. Tras completarlos, ejecutaremos `jekyll build`, haremos un push a nuestro repositorio de GitHub y solicitaremos un pull request a este repositorio.

### ¿Cómo crear un nueva actividad?

Para crear una nueva actividad, debes copiar unas de las plantillas (preferiblemente `ejemplo-jsonlp`) del directorio `_drafts` y nombrar el fichero siguiendo el esquema de fecha+nombre, como en el resto. Por ejemplo:

```
2015-12-05-actividad-ejemplo.md
```

Para poder ver los borradores en el servidor local, deberás ejecutar Jekyll en modo draft con `jekyll serve --drafts`.

Los post de actividad se maquetan mediante markdown. Adjuntamos [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Una vez hayas terminado la actividad y quieras _publicarla_, símplemente debes moverla a la carpeta `_posts`.

```
├── _posts
│   ├── 2015-12-05-actividad-ejemplo.md
```

Una vez esté en publicada en actividades, el sistema **creará automáticamente un post en la categoría de actividades.** Tras ello, seguiremos el proceso de build - push - pull request explicado anteriormente.

### To-do list

 * Modificar Readme.
 * Links RRSS.
 * Modificar aviso legal.
 * Modificar página 404.
 * Configurar Google Analytics.
 * Modificar o borrar gaug.es. 
 * Modificar metatags Twitter card en default.html.
 * Títulos de las páginas.
 * Modificar contenido index.html.
 * Modificar _config.yml.
 * Link en portada a blog.
 * Modificar URL en post, post*jsonld y post*jsonld*varios*dias.
 * Configurar calendario en Actividades.
 * Modificar aviso legal.
 * Eliminar favicon en /css.
 * Elegir color principal y cambiar en style.css (al final).
 * Enlace a foro en portada.
 * Modificar atom y sitemap.
 * Tests con travis-CI.

### Licencia

© HackLab Almería y respectivos autores 2015.
© [Indavelopers](http://www.indavelopers.com), Grupo de Usuarios de R Almería y respectivos autores 2015.
Licencia [Attribution 4.0 International (CC BY 4.0)][5]  
[![Attribution 4.0 International (CC BY 4.0)](http://i.creativecommons.org/l/by/4.0/88x31.png "Attribution 4.0 International (CC BY 4.0)")][5]

[1]: http://jekyllrb.com
[2]: http://es.wikipedia.org/wiki/Markdown
[3]: http://jekyll-windows.juthilo.com
[4]: http://railsapps.github.io/xcode-command-line-tools.html
[5]: http://creativecommons.org/licenses/by/4.0/
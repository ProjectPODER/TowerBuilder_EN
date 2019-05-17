# Editing texts

Editable text files are in MarkDown (.md) format.

Markdown is a light and user-friendly syntax used to style web texts. You are in control of the document visualization: you can bolden or italicize text, add images and create lists, among other things that can be done with MarkDown. Broadly speaking, Markdown is just plain text with some non-alphabetical characters, such as `#` or `*`.

We recommend reading [Github's Markdown guide](https://guides.github.com/features/mastering-markdown/) to learn more about it.

## Main texts

Main texts are composed of sections that appear on the main menu.

To edit files:

1. On GitHub's repository, click on the title of the file you want to modify.
2. Click on the pencil icon located on the upper right corner (Edit this file).
3. Edit the text using Markdown format.
4. Once finished, go to the **Commit changes** section, underneath the edit section. Add a short description of changes you've made on the first box and, optionally, a longer description in the second box. 
5. Save changes by clicking the green **Commit changes** button.

List of editable documents:

To edit texts on the Home page:
  - **1-home.md**

To edit texts in the About page:
  - **4-about.md**

To edit texts on each slide:
  - **collections/_first-slider/slide-1.md**
  - **collections/_first-slider/slide-2.md**
  - **collections/_first-slider/slide-3.md**

To add or remove a slide, just add or remove an **.md** file inside **_first-slider** folder.

If you want to change or add an image (.jpg, .png or .svg) inside the slider, you should add the image inside the **assets/img/** folder and add the file's name to the file corresponding to the slide where images will be.

```
---
title: First Slide
**image: graphic-example.png** -> file's name will be here.
---
```

To edit the visualization slider captions:
  - **collections/_visualization-slider/slide-1.md**
  - **collections/_visualization-slider/slide-2.md**
  - **collections/_visualization-slider/slide-3.md**


### Page names and permalinks

You can edit the name and permalink of each section that will be shown on the main menu.

To do this, find and edit this part:

```
---
layout: home
title: Home
permalink: /
---
```

To change the page's name, edit:

```
---
title: Page name
---
```

To change the permalink, edit:
```
---
permalink: /page-link/
---
```

### Changing the order of items on the main menu

Since TowerBuilder adds items to the main menu in alphabetical order, a custom order can be achieved by editing the numbers at the start of each file name.

This is the default order:

1. home
2. slider.html
3. visualization-slider.html
4. contracts.html
5. posts.md
6. about.md
7. styleguide.md

These are the steps to edit the name of a GitHub file:

1. On GitHub's repository, click on the title of the file you want to modify.
2. Click on the pencil icon located on the upper right corner (*Edit this file*).
3. Edit the filename at the filename box, located above the edit section.
4. Once finished, go to the **Commit changes** section, underneath the edit section. Add a short description of changes you've made on the first box and, optionally, a longer description in the second box.
5. Save changes by clicking the green **Commit changes** button.

**Note:** Note: If you want to remove Style guide page from menu, you need to go to *_config.yml* configurations file and write the file's full name on the exclude section. It should be like this:

```
exclude:
  - Gemfile
  - Gemfile.lock
  - node_modules
  - update_boostrap.sh
  - vendor/
  - docs/
  - 7-styleguide.md
```

### Agregar un elemento del menú

Puedes crear un archivo donde podrás añadir texto y aparecerá dentro del menú.

Los pasos para crear un archivo son:

1. En GitHub, navega a la página principal del repositorio.
2. En el repositorio, busca la carpeta donde deseas crear un archivo.
3. Encima de la lista de archivos, haz clic en _Create new file_.
   ![](https://help.github.com/assets/images/help/repository/create_new_file.png)

4. En el campo de _Name your file_, escribe el nombre y la extensión del archivo. Para crear subdirectorios, escribe el /separador de directorios.
   ![](https://help.github.com/assets/images/help/repository/new-file-name.png)

5. En la pestaña _Edit new file_ , agrega contenido al archivo.
6. Es importante agregar siempre a los archivos nuevos creados, el siguiente código al incio del archivo:
   ```
   ---
   layout: page -> siempre debe ser **page**
   title: Nombre de la página -> puedes cambiar al título que desees
   permalink: /nombre-del-link/ -> puedes cambiar al nombre del link que desees mostrar
   ---
   ```
7. Para revisar el nuevo contenido, haz clic en _Preview_.
   ![](https://help.github.com/assets/images/help/repository/new-file-preview.png)

8. Al final de la página, en el primer campo de la sección **Commit new file**, añadir una corta descripción de los cambios que se hicieron, puedes agregar una descripción más extensa en el siguiente campo, de manera opcional.
9. Guardar los cambios dando click en el botón verde **Commit new file**.

Para información más detallada de cómo crear un nuevo archivo, visita la [documentación oficial de Github](https://help.github.com/en/articles/creating-new-files).

### Eliminar un elemento del menú

Para quitar un elemento del menú, basta con eliminar el archivo. 

Para eliminar un archivo en Github:

1. Da click en el archivo que quieres eliminar.
2. En la parte de arriba del documento, da click en el ícono del bote de basura.
3. Al final de la página, en el primer campo de la sección **Commit changes**, añadir una corta descripción de los cambios que se hicieron, puedes agregar una descripción más extensa en el siguiente campo, de manera opcional.
5. Guardar los cambios dando click en el botón verde **Commit changes**.


## Artículos

Los artículos son notas que analizan contratos, y aparecen vinculados a estos en el gráfico.


### Crear un artículo

Para crear un artículo, en tu repositorio, ve dentro de la carpeta **_posts** que a su vez está dentro de **collections**.

Da click en **Create new file**.

Escribe dentro del campo **Name your file** el nombre del nuevo archivo, que debe tener el siguiente formato, de lo contrario, Tower Builder no podrá leer el artículo:

```
YEAR-MONTH-DAY-title.MARKUP
```

Donde **YEAR** tiene un número de cuatro dígitos, **MONTH** y **DAY** tienen números de dos dígitos, y **MARKUP** es la extensión del archivo que representa el formato utilizado. Por ejemplo, los siguientes son ejemplos de nombres válidos:

```
2018-12-31-new-years-eve-is-awesome.md
2018-09-12-how-to-write-a-blog.md
```

Todos los archivos de los artículos, deben comenzar con el siguiente encabezado:

```
---
layout: post -> Siempre debe ser post
title:  "Welcome to Jekyll!" -> Puedes cambiarlo por el nombre que desees para tu artículo.
author: "Name" -> Puedes escribir el nombre del autor del artículo
---
```

Debajo del encabezado, puedes seguir con el contenido del artículo, siguiendo el mismo formato de los demás textos editables, que es Markdown.

Para que se puedan vincular con el gráfico, debes saber el identificador del contrato OCID y agregarlo en el encabezado del  archivo, de la siguiente manera:

```
person: Juan Carlos Dueño
```

Para guardar el nuevo archivo, da click en el botón **Commit new file** después de agregar un comentario sobre el nuevo archivo.

Si deseas conocer todas las opciones posibles para los encabezados de los artículos y más configuraciones relacionadas, [visita este link](https://jekyllrb.com/docs/posts/).

**Importante:** Todas las modificaciones se reflejan automáticamente en el sitio público, este proceso puede tardar varios minutos para verse en la web.

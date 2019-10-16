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

To edit texts on the About page:
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

Since TowerBuilder adds items to the main menu in alphabetical order, a custom order can be achieved by editing the numbers at the start of each file's name.

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
3. Edit the name in the filename box, located above the edit section.
4. Once finished, go to the **Commit changes** section, underneath the edit section. Add a short description of changes you've made on the first box and, optionally, a longer description in the second box.
5. Save changes by clicking the green **Commit changes** button.

<!-- **Note:** If you want to remove Style guide page from menu, you need to go to *_config.yml* configurations file and write the file's full name on the exclude section. It should be like this:

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



### Add an item to menu

You can create a file where you can add text and it will appear inside the menu.

Steps to create a file are:

1. In GitHub, go to the repository's home page and open the folder where you want to create a file.
2. Click on  _Create new file_, located above the upper-right corner of the file list.
![](https://help.github.com/assets/images/help/repository/create_new_file.png)
3. On  _Name your file_ box, write the file's name with its extension. Use the forward slash (/) to create subdirectories.
   ![](https://help.github.com/assets/images/help/repository/new-file-name.png)
4. Write the contents of the file in the _Edit new file_ tab.
5. Always add the following file's start code to new files created:
   ```
   ---
   layout: page -> must always be **page**
   title: Page name -> the title you chose for the page
   permalink: /link-name/ -> change it for the link you want to show
   ---
   ```
6. To review the content, click on _Preview_.
   ![](https://help.github.com/assets/images/help/repository/new-file-preview.png)
7. Once finished, go to the **Commit New File** section, underneath the edit section. Add a short description of changes you've made on the first box and, optionally, a longer description in the second box.
8. Save changes by clicking the green **Commit changes** button.

For more in-depth information of how to create a new file, visit [Github's official documentation](https://help.github.com/en/articles/creating-new-files).

### Delete a menu item

Removing a menu item is easy, you just need to delete its file. 

If you want to delete a GitHub file:

1. Click on the file you want to delete.
2. On the upper part of the document, click on the trash can icon.
3. At the end of the page, add a short description of changes to **Commit new file**, the section's first box. You can optionally add a longer description in the following box.
5. Save changes clicking on the green **Commit changes** button. -->

### Add a new page

To add a new page, you can create a file where you can add text in markdown format.

Steps to create a file are:

1. In GitHub, go to the repository's home page and open the folder where you want to create a file.
2. Click on  _Create new file_, located above the upper-right corner of the file list.
![](https://help.github.com/assets/images/help/repository/create_new_file.png)
3. On  _Name your file_ box, write the file's name with its extension.
   ![](https://help.github.com/assets/images/help/repository/new-file-name.png)
4. Write the contents of the file in the _Edit new file_ tab.
5. Always add the following file's start code to new files created:
   ```
   ---
   layout: page -> must always be **page**
   title: Page name -> the title you chose for the page
   permalink: /link-name/ -> change it for the link you want to show
   ---
   ```
6. To review the content, click on _Preview_.
   ![](https://help.github.com/assets/images/help/repository/new-file-preview.png)
7. Once finished, go to the **Commit New File** section, underneath the edit section. Add a short description of changes you've made on the first box and, optionally, a longer description in the second box.
8. Save changes by clicking the green **Commit changes** button.

For more in-depth information of how to create a new file, visit [Github's official documentation](https://help.github.com/en/articles/creating-new-files).


### Add a menu item

When creating a new page that contains the header described above, it will automatically be added to the bottom of the menu.

If you want to change the order that the page should appear in the menu, place the corresponding number and modify the numbers of the elements that are already there. To rename a file, follow the [Github documentation here](https://help.github.com/en/articles/renaming-a-file).


### Hide/Delete a menu item

Removing a menu item is easy, you just need to delete its file. 

If you want to delete a GitHub file:

1. Click on the file you want to delete.
2. On the upper part of the document, click on the trash can icon.
3. At the end of the page, add a short description of changes to **Commit new file**, the section's first box. You can optionally add a longer description in the following box.
5. Save changes clicking on the green **Commit changes** button.

If you want to exclude a page from the menu, but not delete the file and offline, you should only add to the header **"published: false"**:

```
---
published: false
permalink: /link/ -> Offline page.
---
```
If you want to exclude the menu item, but keep the page online, you must delete the header title:

```
---
layout: page
title: Page name -> Delete this line.
permalink: /link/ -> Online page
---
```

**Note:** With these options, you can hide or delete any section like the Slider, the Visualization or the Styleguide page of your final project.

### Edit the More information menu button title

To change the button title that appears when you reduce the screen width, you only have to change the text in the file **_ config.yml** of the next variable:

```
menu_button_title: More information -> change it to the text you want
```

### Edit the Contracts page titles

You can change the different filter titles of the contract search page and the table columns titles in the file **_ config.yml**, this is an example of the default configuration:

```
contracts_title: Contracts by companies
search_title: Search
search_placeholder: Enter keyword to search
amount_title: Total amount (Mexican pesos)
amount_from_placeholder: From $
amount_to_placeholder: to $
type_contract_title: Type of contract
type_contract_title_tooltip: The law requires that the Buyer defines the type of contract because the rules vary in each case.
type_contract_all_option: All
type_procedure_title: Type of procedure
type_procedure_title_tooltip: La licitación pública es según la ley mexicana el procedimiento adecuado para contratar obra publica. Excepcionalmente también se pueden realizar otro tipo de procedimientos como adjudicación directa, convenio e invitación a cuando menos tres proveedores.
type_procedure_all_option: All
date_range_title: Date range
date_range_from_placeholder: From
date_range_to_placeholder: to
date_range_title_tooltip: Find active contracts between two dates.
filter_footnote_title: Apply filters on contracts with companies.

# Customize the Contract table titles
column_1: Companies
column_2: No. of contracts
column_3: Total amount
```

## Articles

Articles are notes that analyze contracts, and are linked to them in the graph.


### Create an article

To post an article in your repository:

1. Go to the **_posts** folder, inside the **collections** folder.

2. Click on **Create new file**.

3. Write the new file's name. TowerBuilder won't be able to read it unless it’s formatted this way:

```
YEAR-MONTH-DAY-title.MARKUP
```

**YEAR** is four-digit, **MONTH** and **DAY** are two-digits;
title: the desired title;
**MARKUP**: file extension

The following names are both valid:

```
2018-12-31-new-years-eve-is-awesome.md
2018-09-12-how-to-write-a-blog.md
```

4. All articles have to start with the following header:

```
---
layout: post -> All articles are post type.
title:  "Welcome to Jekyll!" -> The name you want for your article.
author: "Name" -> The author's name for your article.
---
```

5. Write the contents of the article. You can format it using Markdown, as in all other editable texts.

6. To link with graphic, you must know its OCID contract identifier, and add it to the header like this:

```
person: Juan Carlos Dueño
```

To save the new file, click on the **Commit new file** button after adding a comment about it.

If you wish to know all possible options for articles headers and other related settings, [visit this link](https://jekyllrb.com/docs/posts/).

**Important:** All modifications are automatically reflected on the public site, although this process may take several minutes to take place.

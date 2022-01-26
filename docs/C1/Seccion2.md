# Edit configuration

Now you can start building your website: you'll have to define a project name and other settings. To do this, you must:

1. Browse to the settings file: To do so, enter your repository and search for the file named "**_config.yml**".

2. Click on the file's name to open it.

3. Click on the "edit" button on the upper-right corner.

4. Start changing values. This file is on a YAML format, which means it's composed of a series of variables and its values. Each line starts with a variable name, and a colon (:) followed by a value.

	```
	variable: value
	```

	Don’t change the names of the variables, only make changes after the “:”.

    - Begin by changing the _title_ variable. It defines your site's name in different places, such as browser's tabs, search results and the header of the site. For this, search where it says:

	```
    title: "TowerBuilder"
	```
    and replace the text between quotation marks with your site’s title:
	```
    title: "South road's contracting analysis".
	```

	- Other important values to change are:

	```
    image: tb-logo.png -> change for the project logo, or leave it empty, it's optional.
    description: >-
  	 Modify the existing text and put your project's description here.
	```

		- To enable or disable the top menu, toggle the following variable between true or false:
    ```
    top_menu: true
    ```

    - To change the title of the top menu item (appears when there are several items in the menu or when the window is adjusted to smaller screens):
    ```
    menu_button_title: More information
    ```

	  To change the logo, follow [these instructions](https://towerbuilder.readthedocs.io/en/latest/C2/Seccion3.html#changing-the-logo).

	- To display the main name of your graphic on the Visualization slider, edit the following variable:

	```
    graphTitle: "Graphic name"
	```

	- Jekyll has a Plugins system that allows executing the customized code without a need to modify the Jekyll's source. In the TowerBuilder’s configuration page, it's represented in the following way:
	```
	plugins:
  	  - jekyll-feed
  	  - jekyll-sitemap
	```

	[In this link](https://jekyllrb.com/docs/plugins/), you can find more advanced information about the plugins.

	- To exclude any file, add it to the **exclude** section.
	```
    exclude:
      - Gemfile
      - Gemfile.lock
      - node_modules
      - vendor/
      - docs/
	```

	- Collections are an excellent way to group related content. This is how our configuration file shows TowerBuilder’s collections:
	```
    collections_dir: collections
    collections:
      first-slider:
        output: true
      visualization-slider:
        output: true
	```

	**Important:** This collections directory shouldn’t be edited. Collections can be added, but without deleting the default ones.

	For more information about collections, [visit this page](https://jekyllrb.com/docs/collections/).

	- The last variables shown into "**_config.yml**" file are related to the options TowerBuilder has in order to show the articles:
	```
    show_excerpts: true
	future: true
	```

	If you want to know more about these options, visit [this link](https://jekyllrb.com/docs/posts/).

If you want to learn about more advanced options of this configuration file, visit [Jekyll's official documentation](https://jekyllrb.com/docs/configuration/options/).


To add analytics to the site, you can add one of these options:

```
# Analytics Configuration
jekyll_analytics:
  GoogleAnalytics:          # Add, if you want to track with Google Analytics
    id: UA-123-456          # Required - replace with your tracking id
    anonymizeIp: false      # Optional - Default: false - set to true for anonymized tracking

  Matomo:                   # Add, if you want to track with Matomo (former Piwik Analytics)
    url: matomo.example.com # Required - url to Matomo installation without trailing /
    siteId: "1234"          # Required - replace with your Matomo site id (Write id as string)

  Piwik:                    # Add, if you want to track with Piwik
    url: piwik.example.com  # Required - url to Piwik installation without trailing /
    siteId: "1234"          # Required - replace with your Piwik site id (Write id as string)

  MPulse:                   # Add if you want to track performance with mPulse
    apikey: XXXXX-YYYYY-ZZZZZ-AAAAA-23456   # Required - replace with your mPulse API key

  Plausible:
    domain: 'example.com'   # The domain configured in plausible
    source: 'https://plausible.example.com/js/plausible.js' # The source of the javascript
```
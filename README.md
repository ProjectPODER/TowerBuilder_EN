# TowerBuilder

TowerBuilder is a website creation tool that doesn't require programming knowledge to create websites featuring contracting data visualization. It's specifically oriented to large public works and it’s inspired by www.torredecontrol.org.

You can find full documentation in [TowerBuilder manual](https://towerbuilder.readthedocs.io/en/latest/), where you’ll find step-by-step instructions on how to use this tool to create your own website.

#### What do I need to create my own TowerBuilder website?
* Get an [OCDS](http://standard.open-contracting.org/latest/en/)-format contracting list..
* Create a spreadsheet shared with contracting businesses owners.
* Write and edit text in [MarkDown](https://www.markdownguide.org/)-format.
* A [GitHub.com](https://github.com/) account.

#### What are the advantages of creating websites using TowerBuilder?
* Default design doesn't require any coding or web hosting, everything is done in GitHub.com.
* Visually impressive data visualization and a useful contracting search system.
* If you already have the data, you'll be able to create your website within minutes.
* Highly customizable design.
* You can use open data from your country's government and show how useful the open contracting standard (OCDS) is for journalism.

#### What are the steps?
1. Fork the repository
2. Edit configuration
3. Import data
4. Edit texts
5. Publish the website

If you find any problem not contemplated in the documentation, or need any help creating your website, you can email PODER: info@quienesquien.wiki. You can also use GitHub’s own issue system: [https://github.com/ProjectPODER/TowerBuilder/issues](https://github.com/ProjectPODER/TowerBuilder/issues).

### Install the development kit
If you're a developer and wish to run TowerBuilder locally, follow these steps:

1. In the terminal, clone the repository:
`   git clone https://github.com/ProjectPODER/TowerBuilder.git`

2. Enter the project:
`   cd TowerBuilder`

3. Once in the folder, install all the needed units for the project:
`   bundle install`

4. Build the website and make it available at localhost:
`   bundle exec jekyll serve`

5. Browse to http://localhost:4000

#### Next steps
- Make Visualization section's graphic optional.
- Allow other kinds of visualizations in this section.

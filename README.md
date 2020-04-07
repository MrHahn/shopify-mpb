# Shopify Monster Page Builder

This is a simple builder that will allow you to build monster pages quickly with a few drag and droppable widgets


### Installing

Install the page template

```
page.monster-page-1.liquid
```

Install the section

```
monster-blocks.liquid
```

Install the snippets

```
monster-block.liquid
monster_content_block.liquid
monster_cta_row.liquid
monster_fifty_fifty.liquid
monster_hero_block.liquid
```

Install the styles

```
monster_styles.css
(the contents of this file can just be copied to the bottom of any .scss stylesheet. .css will not work)
```

once all files have been added to the theme you just need to add this snippet of code to theme.liquid file above the </head> tag
```
  {% assign template_name = template.suffix | split: '-' %}
  {% if template_name[0] == 'monster' %}
  	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
  {% endif %}
```
This will ensure that the page that is using the builder will have bootstrap4 available for the grid.





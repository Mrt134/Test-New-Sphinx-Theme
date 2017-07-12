#TrueOS Style 

###A Custom Sphinx theme for iX documentation.

#The trueos_style is intended for use in the various iX Systems
documentation which uses the Sphinx Documentation Generator:
https://www.sphinx-doc.org/

**Simple instructions to add and activate trueos_style:**

* Create a [themes] directory in the base directory of the Sphinx project.
* Copy the entire trueos_style directory into the new [themes] directory.
* Edit the project conf.py file and alter **html_theme =** to read:

```
 html_theme = 'trueos_style'
```

* Be sure Sphinx knows the path to the custom theme:

```
  html_theme_path = ['themes']
```

# Test-New-Sphinx-Theme
Building a new efficient Sphinx theme for iX Sphinx projects.

There are four themes available for experimentation, housed in the `_themes` directory.
1. **sphinx_rtd_theme** is the currently available Read the Docs theme, and is to be used for copies/reference only.
2. **trueos_style** is the current theme used for most iX Sphinx documentation, and is to be used for copies/reference only.
3. **new_trueos_style** is an experimental theme that uses *trueos_style* as references for a blank stylesheet.
   This can be manipulated/deleted/reworked freely.
4. **modify_rtd_theme** is an experimental theme that copies *sphinx_rtd_theme* and attempts to import custom values from
   *trueos_style*. Primary experimentation theme.

**CLI instructions:**

Type `make html` in the directory with the *Makefile* to build the test Sphinx doc.
Type `firefox _build/html/index.html &` to open the Sphinx doc in a new Firefox tab.
Type `make clean` to remove all built files. Use `make clean` before `make html` to rebuild the html files with any .css/html
style changes.

**Changing themes**
Open **conf.py** file.
Find the `html_theme = '[THEME]'` line.
Adjust `[THEME]` to any of the other themes housed in the `_themes` directory. Keep the surrounding ['] symbols.
Run `make clean` and `make html` to build the docs with the new theme.

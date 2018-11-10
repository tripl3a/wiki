# Jupter

## Lab

If you use `conda`, you can install it with:
```
conda install -c conda-forge jupyterlab
```

Start JupyterLab using:
```
jupyter lab
```

Documentation: https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html

Extensions: 
* https://github.com/mauhai/awesome-jupyterlab
* https://medium.com/@subpath/jupyter-lab-extensions-for-data-scientist-e0d97d529fc1

## Slides

Run for example:  
```
jupyter nbconvert <notebook_title>.ipynb --to slides --post serve
```

With a theme:
```
jupyter nbconvert <notebook_title>.ipynb --to slides --post serve --SlidesExporter.reveal_theme=white
```

With [output toggle](http://www.damian.oquanta.info/posts/hide-the-input-cells-from-your-ipython-slides.html): 
```
jupyter nbconvert <notebook_title>.ipynb --to slides --post serve --template output_toggle
```

## Extensions

Install the optional extensions:
```
conda install -c conda-forge jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
```

## nbviewer

A simple way to share Jupyter Notebooks. Enter the location of a Jupyter Notebook to have it rendered.  
https://nbviewer.jupyter.org/  

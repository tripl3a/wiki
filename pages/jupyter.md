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

## Slides

Run for example:  
```
jupyter nbconvert 07_ensemble_learning_and_random_forests-part2.ipynb --to slides --post serve --template output_toggle
```

With a theme:
```
jupyter nbconvert <notebook_title>.ipynb --to slides --post serve --SlidesExporter.reveal_theme=white --template output_toggle
```

Output toggle: http://www.damian.oquanta.info/posts/hide-the-input-cells-from-your-ipython-slides.html

## Extensions

Install the optional extensions:
```
conda install -c conda-forge jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
```
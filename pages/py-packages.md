# Python package management

## Conda

Create and activate a new environment named `myenv`:
```
conda create -n myenv
source activate myenv
```

Delete environment:
```
TODO
```

Install multiple packages (argument `-y` to omit the prompts):
```
conda install -y numpy matplotlib scikit-learn
# with specific versions:
conda install -y seaborn==0.8.1 numpy==1.14.5 pandas==0.23.1 scikit-learn==0.19.1
```

## Jupyter

To make the virtual environment available within jupyter:  
```
source activate myenv
conda install -y ipykernel
ipython kernel install --user --name=myenv
```

Delete jupyter kernel:
```
TODO
```

## Packages from Git

Install a package from GitHub:

```
pip install git+https://github.com/jkbr/httpie.git
```
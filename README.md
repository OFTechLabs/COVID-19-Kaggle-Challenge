[PROJECT NAME]

==============================

this toolbox allows for analysis of [...]

### Installing

1. run SetupPackage.ps1
 - build python virtual environment
 - install python dependencies
 - install python package
 
 
```
.\SetupPackage.ps1
```

Note: one might need to set the execution policy of powershell by running the command below from an administrator powershell: 

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
```



### Generate License
When new packages are added one needs to run this script and commit the new 'License.md' in order to remain compliant with our internal processes
1. run SetupLicense.ps1
 - generates License.md

```
.\SetupLicense.ps1
```

### Run notebooks

first activate virtual environment:


```
# Activate virtual environment
& ./venv/Scripts/activate.ps1
```

got to notebooks:
```
cd .\notebooks
```
and start the jupyter server:
```
jupyter notebook
```



Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
        ├── __init__.py    <- Makes src a Python module
        │
        ├── data           <- Scripts to download or generate data
        │   └── make_dataset.py
        │
        ├── features       <- Scripts to turn raw data into features for modeling
        │   └── build_features.py
        │
        ├── models         <- Scripts to train models and then use trained models to make
        │   │                 predictions
        │   ├── predict_model.py
        │   └── train_model.py
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations
            └── visualize.py
 


--------


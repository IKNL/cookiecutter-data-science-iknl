<img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/iknl_nl.png?raw=true" width=200 align="right">

# Cookiecutter Data Science at IKNL

This is a Cookiecutter template for Data Science projects at IKNL. It is based on the [template by Sven van der Burg](https://github.com/svenvanderburg/cookiecutter-data-science) (you can see the [original project's homepage here](http://drivendata.github.io/cookiecutter-data-science/)).

### Steps to use the Cookiecutter template:
-----------

1. Create a new environment (for example, using [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands)). Make sure that it uses Python 2.7 or >=3.5 (much, much more preferred)
2. Install [Cookiecutter package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0.

Using conda:

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```

or

Using pip:
``` bash
$ pip install cookiecutter
```
3. Open a command prompg (with admin rights) and go to the directory where your project will be created.
4. Then, type

   ``` bash
   cookiecutter https://github.com/arturomoncadatorres/cookiecutter-data-science-iknl
   ```
5. Fill in the required questions (pretty straightforward).
6. Start tracking your project with Git (optional, but much recommended)
7. DONE!



### The resulting directory structure
------------

The directory structure of your new project looks like this:

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
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
│   └── documents      <- Articles, written reports, etc.
│      └── paper       <- LaTeX template for a paper
│   └── figures        <- Generated graphics and figures to be used in reporting
│   └── posters        <- Typically for conferences
│   └── presentations  <- Usually PowerPoints (and their corresponding PDF)
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── results            <- Intermediate/preliminary results (figures, variables, etc.).
│
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.testrun.org
```

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests

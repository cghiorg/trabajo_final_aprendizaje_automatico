Trabajo Final Aprendizaje Automatico
==============================

Predicción de Opiniones sobre el Aborto

Objetivo del Trabajo
El objetivo de este proyecto de aprendizaje automático es desarrollar un modelo que permita predecir las opiniones de las personas sobre el aborto utilizando datos demográficos. Específicamente, se pretende determinar si una persona está a favor o en contra del aborto, o si no tiene una opinión definida, en función de variables como el sexo, la edad, la ocupación y el nivel de educación. El enfoque es comprender cómo estas características demográficas influyen en las opiniones sobre el aborto y proporcionar información valiosa para la toma de decisiones y políticas públicas relacionadas con este tema.

Contexto y Relevancia del Problema
El tema del aborto es una cuestión altamente relevante en la sociedad y la política. Las opiniones sobre el aborto están fuertemente influenciadas por factores demográficos, como el género, la edad, la ocupación y el nivel de educación. La toma de decisiones informada en políticas públicas relacionadas con el aborto requiere una comprensión profunda de cómo estas variables impactan en las opiniones.

El contexto en el que se encuentra este problema es especialmente importante debido a los debates y controversias en curso en muchas regiones del mundo sobre la legalización y regulación del aborto. Los gobiernos y las organizaciones de salud pública necesitan una comprensión precisa de las opiniones de la población y de los factores que influyen en esas opiniones para tomar decisiones informadas y promover políticas basadas en evidencia.

Preguntas de Investigación e Hipótesis
El proyecto se centra en responder a la siguiente pregunta de investigación:
¿Es posible predecir con precisión las opiniones sobre el aborto a partir de estas variables demográficas?
La hipótesis subyacente es que las variables demográficas seleccionadas tendrán un impacto significativo en las opiniones sobre el aborto. Se espera que ciertos grupos demográficos tengan una mayor probabilidad de estar a favor o en contra del aborto, y que el modelo de aprendizaje automático pueda capturar estas relaciones para realizar predicciones precisas.

Documento de Datos :doc:`docs/datos.rst`


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
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

# Predicción de enfermedades respiratorias en la Provincia de Tierra del Fuego
==============================
## Contexto del problema
Tierra del Fuego, ubicada en el extremo austral de Argentina, presenta condiciones climáticas 
extremas, con temperaturas frías durante gran parte del año y limitada accesibilidad a centros 
urbanos y de salud. Estas características generan una alta vulnerabilidad frente a enfermedades 
respiratorias, especialmente en poblaciones sensibles como niños y adultos mayores. Anticipar la 
cantidad de casos semanales permite optimizar la distribución de insumos, personal médico y 
camas hospitalarias, evitando saturaciones del sistema sanitario.

## Objetivos específicos
-Identificar patrones temporales y estacionales de enfermedades respiratorias. 

-Detectar semanas críticas en cuanto a número de casos.

-Evaluar qué grupos etarios y enfermedades presentan mayor incidencia estacional.

-Probar distintos modelos de Aprendizaje Automático y comparar su rendimiento.

-Mejorar la planificación y prevención sanitaria mediante predicciones automatizadas.

## Características del Dataset

Se utilizará un dataset nacional obtenido de la página datos.salud.gob.ar que incluye registros de enfermedades respiratorias por provincia entre los años 2022 y 2024. Para este proyecto, se va a filtrar exclusivamente la información correspondiente a Tierra del Fuego, dejando un total de 3135 registros.

Las variables son las siguientes:

***departamento_id***: id del departamento.

***departamento_nombre***: nombre del departamento (Río Grande, Ushuaia).

***provincia_id***: id de la provincia.

***provincia_nombre***: nombre de la provincia.

***año***: año de registro de los casos.

***semanas_epidemiologicas***: identifica la estacionalidad.

***evento_nombre***: nombre de la enfermedad respiratoria.

***grupo_edad_id:*** id del grupo etario.

***grupo_edad_desc***: rangos etarios.

***cantidad_casos***: cantidad de casos registrados.


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

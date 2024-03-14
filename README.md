books_recommendation
==============================

Recommendation of books based on this dataset: https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?select=Ratings.csv

├── notebooks:
                1.0-zupr-data_preparation.ipynb
                    - uploading and cleaning the data
                    - saving cleaned data
                    
                1.1-zupr-data_analysis.ipynb
                    - merging the data 
                
                1.2-zupr-data_visualization.ipynb
                    - visualization of some information from the data
                    
                2.0-zupr-recommendation1.0.ipynb
                    - recommendation system based on the users, that also liked given book
                
                2.0-zupr-recommendation1.1.ipynb
                    - recommendation system based on the users, that also liked given book with rating function that should also consider the same book with different ISBN and in different language
                    - not working, running to long
                    
                2.0-zupr-recommendation1.2.ipynb
                    - recommendation system based on the users, that also like given book with rating function should also consider the same book with different ISBN, but in the same language
                    - not working, running to long
                    
                2.0-zupr-recommendation2.0.ipynb
                    - recommendation system based on the correlation of the rating values from the users of the books
                    - working only on a small sample, not working for all data due need of space for the correlation matrix
                    
                2.0-zupr-recommendation2.1.ipynb
                    - recommendation system based on cosine similarity of the rating values from the users of the books
                    - not working
                    
                2.0-zupr-recommendation3.0.ipynb
                    - recommendation system based on cosine similarity of users

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




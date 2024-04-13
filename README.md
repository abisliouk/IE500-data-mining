# Song genre predictor based on Spotify data

The goal of this project is to create a classifier and see how accurately it can predict song genres. Taking a dataset from Spotify [Pandya, 2022], which is al- ready using machine learning algorithms for these purposes, can help assess if the resulting model can be considered apt for a large-scale business or is more appropriate for a smaller audio streaming market player.

## Structure

The contents of the repository are the following:
### Folders
* [data/](data/) &rarr; datasets used for this project
    - [spotify_data](data/spotify_data.csv): the original [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)
    - [spotify_clean](data/spotify_clean.csv): dataset without only one genre assigned to each song (generated by using the [data-cleaning](data-cleaning.ipynb) notebook)
    - [spotify_simplified](data/spotify_simplified.csv): dataset with only 18 unique genres in total (generated by using the [clustering](clustering.ipynb) notebook)
    - [data_report](data/data_report.html): exploratory data analysis for the original dataset
* [figures/](figures/) &rarr; figures generated for the presentation and report (generated using the [plots](plots.ipynb) notebook)
* [ml_methods/](ml_methods/) &rarr; notebooks with different machine learning algorithms explored for the project

### Notebooks
* [baseline](baseline.ipynb) &rarr;  implement the majority and rule-based baselines
* [clustering](clustering.ipynb) &rarr;  reduce the number of genres in the dataset to only 18 via a combination of agglomerative clustering and manual input
* [data-cleaning](data-cleaning.ipynb) &rarr;  choose only one genre for every song in the dataset that appeared with multiple genres
* [data-exploration](data-exploration.ipynb) &rarr; visualize the features of the dataset and propose preprocessing steps
* [hyperparemter-optimization](hyperparam-optim.ipynb) &rarr; hyperparameter optimization implemented using GridSearchCV
* [plots](plots.ipynb) &rarr; generate plots for the report and presentation


## Setup
1. Activate your virtual environment
2. Run the following command to install all the dependencies needed for this project:
```
pip install -r requirements.txt
```
3. Inspect the code for the different algorithms that were explored (stored under [ml_methods/](ml_methods/]))

## Submission details
Team 1
- Elizaveta Nosova (1983805)
- Miguel Samaniego (1980439)
- Nico Sharei (1986818)
- Julian Ament (1981511)
- Artem Bisliouk (1978986)
- Jannik Kranz (1981766)

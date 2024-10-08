# Cookiecutter Data Science

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

This project template is modified version of the [Cookiecutter Data Science](https://cookiecutter-data-science.drivendata.org/) template, adapted to fit specific needs and made available as a GitHub template.

## Installation
To set up the project structure on your local machine, follow these steps:
### 1. Create a New Repository from the Template
Click on the `Use this template` button located above the code listing and create your repository as usual.
### 2. Clone Your New Repository
Open your terminal and run the following commands:
```
git clone [your-repository-url]
cd [your-repository-name]
```
Replace `[your-repository-url]` with the URL of your new repository and `[your-repository-name]` with the name of your repository.
    
### 3. Adjusting `.gitignore`
Since this is a template, the `/data/` folder is commented out and data will not be exlucded from source control. You should exclude the `data` folder if it contains sensitive data or large files that you don’t want to track in version control. To do it, simply uncomment the `/data/` line by removing the `#`:
```
# Data
/data/
```
Save the `.gitignore` file to prevent the data from being committed to your repository.

## Project Organization
```
├── asserts            <- Static assets such as images, logos, demo data, or other resources used in the project
│
├── data
│   ├── external       <- Data from third party sources
│   ├── interim        <- Intermediate data that has been transformed
│   ├── processed      <- Final, cleaned data ready for modeling
│   └── raw            <- Original, unmodified data dumps
│
├── models             <- Trained and serialized models, model predictions, and evaluation summaries
│
├── notebooks          <- Jupyter notebookswith naming conventions: a number, creator’s initials, and a brief description, e.g.,
│                         `1.0-jqp-initial-data-exploration`
│
├── references         <- Documentation such as data dictionaries, manuals, and all other explanatory materials
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── src                         <- Source code for the project
│   │
│   ├── __init__.py             <- Makes `src` a Python module
│   │
│   ├── configs                 <- Configuration files and variables for the project
│   │   ├── __init__.py 
│   │
│   ├── data                    <- Scripts for data ingestion and preparation
│   │   ├── __init__.py
│   │
│   ├── features                <- Scripts to generate and engineer features for modeling
│   │   ├── __init__.py
│   │   
│   ├── modeling                
│   │   ├── __init__.py 
│   │   ├── predict.py          <- Scripts for running inference with trained models           
│   │   └── train.py            <- Scripts for training models
│   │
│   ├── utils                   <- Utility scripts providing supporting functions to optimize and simplify the main codebase
│   │
│   └── services                <- Service classes to connect with external platforms, tools, or APIs
│       └── __init__.py 
│
├── LICENSE            <- Open-source license if one is chosen
│
├── README.md          <- Top-level README for developers using this project
│
├── requirements.txt   <- File containing the dependencies needed to reproduce the environment,
│                         generated with `pip freeze > requirements.txt`
```
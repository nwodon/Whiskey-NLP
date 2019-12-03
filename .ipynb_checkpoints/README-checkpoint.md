## Table of contents
* [Overview](#overview)
* [Dataset Link](#datasetlink)
* [Articles Consulted](#articlesconsulted)
* [Repository Organization](#repositoryorganization)
* [Technologies](#technologies)
* [Packages](#packages)

# Overview

This repository was created as part of a long term project for a Brown University Graduate Class: Data 1030 taugt by Andras Zsom.

Whiskey is a popular beverage consumed in the United States, with a number of different styles and types. Due to the large diversification of the whiskey market, the beverage can be sold at many price points.

The original dataset of 2.247 observations contained the following features: ID, name, category, review score, price, currency, and description. Note that the currency (all prices were in US dollars) and ID feature did not provide any relevant information. The name and description were text features, category was a categorical feature with 5 different whisky types, and review score and price were continuous features.

The goal of this repository is to explore the relationship between whisky price and other whisky characteristics such as whisky age while using natural language processing.  More precisely, the objective is to develop a predictive whisky price model using different ML techniques. Given that the dataset is feature poor, many of the whisky features were generated through the use natural language processing on the whisky name and description. 

Note that the models that predicted whisky price did not perform well due to the highly skewed nature of the data and so log price was used instead as the target. While many of the features extracted provided valuable insight and helped improve the R2 score of the model, they were generated and/or categorized by referencing whisky articles (see links below). Next steps to improve this model would include more thoroughly exploring the generated features instead of relying on sources on whether or not to add a given whisky brand or implement an whisky age cutoff.

# Dataset Link:

https://www.kaggle.com/koki25ando/22000-scotch-whisky-reviews

# Articles Consulted:

https://www.dmarge.com/2019/02/whiskey-brands.html

https://www.mensjournal.com/food-drink/the-50-best-whiskeys-in-the-world-w211382/monkey-shoulder-blended-malt-scotch-w211406/

https://www.gq.com/story/why-your-whiskeys-age-matters

# Repository Organization:

├── Data/ 
|
├── Figures/ 
|
├── Results/  
|
├── Reports/ 
|
├── Src/ 
|
├── LICENSE 
|
└── README.md 

Raw and Preprocessed data files are in /Data

All generated figures are in /Figures

Model Results (predictions, saved models, etc) are in /Results

Report and Midterm Proposal (pdf versions) are in /Reports

Source codes (ipython notebooks or python files) are in /Src 

# Technologies 

Python 3.7

# Packages Used in Analysis: 

nltk==3.4.5

pandas==0.25.0

perfplot==0.6.8

pickleshare==0.7.5

plotly==4.1.1

plotly-express==0.4.1

scikit-image==0.15.0

scikit-learn==0.21.3

scipy==1.3.1

seaborn==0.9.0

statsmodels==0.10.1

sympy==1.4

textcleaner==0.4.26

numpy==1.17.1

matplotlib==3.1.1

regex==2019.11.1

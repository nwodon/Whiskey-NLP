# Whiskey-NLP

This repository was created as part of a long term project for a Brown University Graduate Class: Data 1030 taugt by Andras Zsom.

Whiskey is a popular beverage consumed in the United States, with a number of different styles and types. Due to the large diversification of the whiskey market, the beverage can be sold at many price points.

The original dataset of 2.247 observations contained the following features: ID, name, category, review score, price, currency, and description. Note that the currency (all prices were in US dollars) and ID feature did not provide any relevant information. The name and description were text features, category was a categorical feature with 5 different whisky types, and review score and price were continuous features.

The goal of this repository is to explore the relationship between whisky price and other whisky characteristics such as whisky age while using natural language processing.  More precisely, the objective is to develop a predictive whisky price model using different ML techniques. Given that the dataset is feature poor, many of the whisky features were generated through the use natural language processing on the whisky name and description. 

Note that the models that predicted whisky price did not perform well due to the highly skewed nature of the data and so log price was used instead as the target. While many of the features extracted provided valuable insight and helped improve the R2 score of the model, they were generated and/or categorized by referencing whisky articles (see links below). Next steps to improve this model would include more thoroughly exploring the generated features instead of relying on sources on whether or not to add a given whisky brand or implement an whisky age cutoff.

The dataset used is linked below:
https://www.kaggle.com/koki25ando/22000-scotch-whisky-reviews

Articles Consulted:
https://www.dmarge.com/2019/02/whiskey-brands.html

https://www.mensjournal.com/food-drink/the-50-best-whiskeys-in-the-world-w211382/monkey-shoulder-blended-malt-scotch-w211406/

https://www.gq.com/story/why-your-whiskeys-age-matters

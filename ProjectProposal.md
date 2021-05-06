# Classification Project

### Predicting Horse Racing Results

For this project, we will set out to explore 
[Hong Kong syndecate horse racing data](https://www.kaggle.com/hrosebaby/horse-racing-dataset-for-experts-hong-kong?select=results.csv) 
to investigate predicting whether or not a horse will place in their upcoming race!


### Question/need:
Hong Kong's Jockey Club is one of the most lucrative horse racing syndectics in the world, attracting more than 17.86 million dollars of bets per race. The purpose of this analysis is to apply this model to future horse races of the Hong Kong's Jockey Club to give the user a statistical edge when placing their bets on a particular horse.

### Data Description:
The dataset will be taken from Kaggle (linked above) which compiles data from the Hong Kong Jockey Club's 2014-2017 season and contains over 14,000 data points. The current data set has more than 15 features readily available, with the possibility of more to be engineered.

The baseline odds of a horse comng in 1st, 2nd, or 3rd in our dataset is around 30%.


Our target will be a binary problem with 0 representing ****not placing**** - coming in 4th place or lower, and 1 representing a horse **placing** - coming in 3rd place or higher.

### Tools:

SQL Lite - for data storage  
Python - for data processing/modeling  
Flask - for potential Web Application to display model  


### MVP:

An MVP for this project will consist of a simple model that can compute - although with not much accuracy - the odds of a horse placing given the information inputed into the model.

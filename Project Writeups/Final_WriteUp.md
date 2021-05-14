Brandon McNeil   
Metis Project 4 - Classification

## Context
Hong Kong's Jockey Club is one of the most lucrative horse racing institutions in the world, attracting more than 17.86 million dollars of bets per race. 

The purpose of this analysis is to apply this model to future horse races of the Hong Kong's Jockey Club to give the user a statistical edge when placing their bets on a particular horse.
 
## Data
The dataset was taken from Kaggle](https://www.kaggle.com/hrosebaby/horse-racing-dataset-for-experts-hong-kong?select=results.csv)  which compiles data from the Hong Kong Jockey Club's 2014-2017 season and contains over 14,000 data points.   

Our target will be a binary problem with 0 representing not placing - coming in 4th place or lower, and 1 representing placing - coming in 3rd place or higher.  

Features created were Horse_Winning (count of horses 1st place wins from last 2 races, if none then 0), Horse_Placing (count of horse coming in 1-3 position from last 3 races, if none then 0), Position_Counter, Weight_Class, Odd_Type, Jockey_Winning, and Jockey_Placing.
 
## Model 

Our final model was a Random Forest Model that with the hyperparameter n_estimators set to 200, max_depth set to 10 and class_weight set to "balanced".

The final ROC AUC score for our model was .77%.

To judge the results of our model, we took the soft probability scores and ranked them from highest to lowest - picking the top 3. Our results varied per race, but predicted at least 2 of the winners for most races.


![image](https://user-images.githubusercontent.com/43186680/118285897-ec2b6a00-b49f-11eb-80aa-967d510fd0df.png)


 
## Tools
Altair for visualizations   
Pandas  
DateTime  
Numpy  
RandomForestClassification  
XGBoost  
LogisticRegression  
SQLite Database  


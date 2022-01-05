# Project_Django
Hello,
In the context of a school project, we were able to carry out the study of drug consumption with the implementation of Machine Learning algorithms coded in Python language.
We work on a dataset about people from all walks of life who answered questions about their drug use. 
We wanted to manipulate this fairly complete dataset in the most relevant way to finally obtain the best predictions and especially to be able, in a final perspective, to make prevention to the youngest about the dangers of drug addictions.
Thus, one of the most important questions concerning the study of our data is how to separate the different types of drug users.
After much consideration, we decided to define a "user" as someone who has used a drug in the last month. "Non-Users" are persons with drug consumption as "Never Used", "Used over a Decade Ago", "Used in Last Decade" and "Used in Last Year".
The data set included information on the consumption of 18 centrals nervous system psychoactive drugs : alcohol, amphetamines, amyl nitrite, benzodiazepines, cannabis, chocolate, cocaine, caffeine, crack, ecstasy, heroin, ketamine, legal highs, LSD, methadone, mushrooms, nicotine, and VSA (output attributes).
We decided to create different categories of drugs based on the correlation pleiades presented in the first article of the website.
Therefore, we have :
-	Heroin pleiad : crack, cocaine, methadone, and heroin
-	Ecstasy pleiad : amphetamines, cannabis, cocaine, ketamine, LSD, magic mushrooms, legal highs, ecstasy and amyl
-	Benzodiazepines pleiad : methadone, amphetamines, benzodizepine and cocaine
-	Accessible drugs pleiad : alcohol and nicotine
After a study about the correlation between features and targets, we decided to keep those features : "Age","Gender","Education","Neuroticism","Extraversion","Openness","Agreeableness","Conscientiousness","Impulsiveness","Sensation".
Therefore, before creating Machine Learning models we split our datas in train and test datas.
We train our models and we have done a lot of GridSearchCV in order to find the best hyperparameters for each models.
After training our models, we plot ROC curves and F1 score in order to compare the efficacity of each model.
Finally, in this way, we find 3 best ML models to predict the consumption of users for Heroin, Ecstasy and Benzo drugs.
Each type of drugs have his own Machine Learning model.
To complete our job, we developed a Django application where you can enter all your attributes. After filling this form, you can click on the button « Check predictions ». 
Then, it will appear your predictions results.
This application reveal our first goal, it could make prevention to the youngest about the dangers of drug addictions.

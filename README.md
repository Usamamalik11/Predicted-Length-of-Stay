![patient](https://user-images.githubusercontent.com/50501366/95576377-c80b3480-0a49-11eb-81fd-971b22e697d8.jpg)

# Predicted Length of Stay at Hospital:
An epidemic has engulfed the whole world. Recent Covid-19 Pandemic has raised alarms over one of the most overlooked area to focus: Healthcare Management. While healthcare management has various use cases for using data science, patient length of stay is one critical parameter to observe and predict if one wants to improve the efficiency of the healthcare management in a hospital.

This parameter helps hospitals to identify patients of high LOS risk (patients who will stay longer) at the time of admission. Once identified, patients with high LOS risk can have their treatment plan optimized to miminize LOS and lower the chance of staff/visitor infection. Also, prior knowledge of LOS can aid in logistics such as room and bed allocation planning.

The purpose of this project is to accurately predict the Length of Stay for each patient on case by case basis so that the Hospitals can use this information for optimal resource allocation and better functioning. The length of stay is divided into 11 different classes ranging from 0-10 days to more than 100 days.
# Data Set:
The dataset has been obtaine from kaggle(link:https://www.kaggle.com/nehaprabhavalkar/av-healthcare-analytics-ii). It was actually a hackathon conducted by Analytics Vidhya(link:https://datahack.analyticsvidhya.com/contest/janatahack-healthcare-analytics-ii/#ProblemStatement).
## Features: 
The dataset comprised of seventeen columns including the stay variable. Lets have a look at some of them.
### Hospital Type Code:
It is a categorical feature and was one hot encoded for use. Hospital type a was the most frequent one among them.
### Hospital Region code:
The most frequent one among them was region X. It was also one hot encoded for use.
### Department:
A categorical feature which showed that gyne patients were in a large number visiting the hospital and were usually the ones to stay for long.
### Ward type:
Ward type R was the most frequent one but it were the patients in ward type S who stayed for long.
### Type of Admission:
A large number of patients suffered from trauma and were usually the ones who stayed for long.
### Severity of Illness:
Surprisingly, patients with moderate severity of illness were the ones who stayed for long as compared to other levels of severity of illness.
### Age:
Patients aged from 40-80 were quite large in number and were the ones who stayed for long as compared to patients of other age groups.

# Model Development and Evaluation:
After normalization, I tried different classification approaches. The ones which gave the best results(which is still a very low accuracy score) were random classification, xgboost classifier and catboost classifier. I also tried the gridsearch cv method but the was unable to achive any significant improvement.
## RandomForest Classifier:
It almost gave the accuracy of 42%.
## XGBoost Classifier:
It also gave the same accuarcy i.e. 42%. The default base estimator was used.
## Catboost Classifier:
It also gave 42% accuracy with the default base estimator.

You are welcome to make any changes to the code and further improve the results.

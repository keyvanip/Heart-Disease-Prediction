# Heart-Disease-Prediction
## I. Abstract
Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 32% of all deaths worldwide [[1]](https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds)). In the United States, about 1 in 4 deaths are caused by CVDs [[2]](https://www.cdc.gov/heartdisease/index.htm). Hence, it is important to detect cardiovascular diseases as early as possible and prevent further complications. In this project, I aim to build and analyze supervised Machine Learning and regression models that can accurately predict heart disease in a sample population. The collected [dataset](https://www.kaggle.com/fedesoriano/heart-failure-prediction) contains 12 features that is used for this classification problem. 

## II. Dataset Description
1. Age: age of the patient [years]
2. Sex: sex of the patient [M: Male, F: Female]
3. ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical 
Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
4. RestingBP: resting blood pressure [mm Hg]
5. Cholesterol: serum cholesterol [mg/dl]
6. FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
7. RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
8. MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]
9. ExerciseAngina: exercise-induced angina [Y: Yes, N: No]
10. Oldpeak: exercise relative to rest(oldpeak), the slope of the peak = ST [Numeric value measured in depression]
11. ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
12. HeartDisease: output class [1: heart disease, 0: Normal]

## III. Methods
In the data exploratory stage, I found no missing values to be present in the dataset; however, I detected two variables that presented incorrect values and those values were adjusted accordingly. Next, I encoded all categorical variables to integer variables to fit and evaluate my Machine Learning models. I then used different visualization techniques to understand the relashionship behaviors between the variables and to determine if the variables exhibit Guassian distribution. Furthermore, I analysed the correlation and multicolinearity between variables, which yielded interesting and thought provoking results. In my final stage, I normalized the variables and trained and tested the selected classifiers using 80/20 train-test split and evaluated the accuracy of each model. The classifiers used in this project are listed below.
1. *Logistic Regression*
2. *Random Forest*
3. *K-Nearest Neighbor*
4. *Gaussian Naive Bayes Classifier*
5. *Gradient Boosting - XGBoost*
6. *Decision Tree*

## IV. Results

In three of the classifiers, we were able to achieve an accuracy of over 90% in a testing set predicting the likelyhood of individuals having a heart disease, while maintaining a low false negative rate.

## V. References
[1] “Cardiovascular Diseases (Cvds).” *World Health Organization, World Health Organization*, https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds). <br />
[2] “Heart Disease.” *Centers for Disease Control and Prevention, Centers for Disease Control and Prevention*, 19 Jan. 2021, https://www.cdc.gov/heartdisease/index.htm. <br />
[3] fedesoriano. (September 2021). *Heart Failure Prediction Dataset*. Retrieved [20 Dec. 2021] from https://www.kaggle.com/fedesoriano/heart-failure-prediction.<br />

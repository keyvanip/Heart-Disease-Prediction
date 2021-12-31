# Heart-Disease-Prediction
## I. Abstract
Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 32% of all deaths worldwide [[1]](https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds)). In the United States, about 1 in 4 deaths are caused by CVDs [[2]](https://www.cdc.gov/heartdisease/index.htm). Hence, it is important to detect cardiovascular diseases as early as possible and prevent further complications. In this project, I aim to build and analyze supervised Machine Learning and regression models that can accurately predict heart disease in a sample population. The collected [dataset [3]](https://www.kaggle.com/fedesoriano/heart-failure-prediction) contains 12 features that are used for this classification problem. 

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

Note: <br />
**ChestPainType**: Typical (classic) angina chest pain consists of (1) Substernal chest pain or discomfort that is (2) Provoked by exertion or emotional stress and (3) relieved by rest or nitroglycerine (or both). Atypical (probable) angina chest pain applies when 2 out of 3 criteria of classic angina are present [[4]](https://www.timeofcare.com/typical-vs-atypical-chest-pain/). <br />
**RestingECG**: The resting electrocardiogram is a test that measures the electrical activity of the heart. Left ventricular hypertrophy (LVH) is a thickening of the wall of the heart's main pumping chamber. This thickening may result in elevation of pressure within the heart and sometimes poor pumping action. The most common cause is high blood pressure[[5]](https://www.mayoclinic.org/diseases-conditions/left-ventricular-hypertrophy/symptoms-causes/syc-20374314). <br />
**ExerciseAngina**: Angina is a type of chest pain caused by reduced blood flow to the heart. Stable angina is usually triggered by physical activity [[6]](https://www.mayoclinic.org/diseases-conditions/angina/symptoms-causes/syc-20369373). <br />
**ST_Slope**: The normal ST segment has a slight upward concavity. Flat, ST segment indicates coronary ischemia, and downsloping, or depressed ST segment is a common manifestation of severe myocardial ischemia. Myocardial ischemia is a medical term for a reduced blood flow in the coronary circulation and is linked to heart disease, and heart attacks [[7]](https://www.mayoclinic.org/diseases-conditions/myocardial-ischemia/symptoms-causes/syc-20375417). 


## III. Methods
In the data exploratory stage, I found no missing values to be present in the dataset; however, I detected two variables that presented incorrect values, and those values were adjusted accordingly. Next, I encoded all categorical variables to integer variables to fit and evaluate my Machine Learning models. I then used different visualization techniques to understand the relationship behaviors between the variables and to determine if the variables exhibit Gaussian distribution. Furthermore, I analyzed the correlation and multicollinearity between variables, which yielded interesting and thought-provoking results. In my final stage, I normalized the variables and trained and tested the selected classifiers using an 80/20 train-test split, and evaluated the accuracy of each model. The classifiers used in this project are listed below.
1. *Logistic Regression*
2. *Random Forest*
3. *K-Nearest Neighbor*
4. *Gaussian Naive Bayes Classifier*
5. *Gradient Boosting - XGBoost*
6. *Decision Tree*

## IV. Results

In three of the classifiers, we were able to achieve an accuracy of over 90% in a testing set predicting the likelihood of individuals having heart disease, while maintaining a low false-negative rate.

## V. References
[1] “Cardiovascular Diseases (Cvds).” *World Health Organization, World Health Organization*, https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds). <br />
[2] “Heart Disease.” *Centers for Disease Control and Prevention, Centers for Disease Control and Prevention*, 19 Jan. 2021, https://www.cdc.gov/heartdisease/index.htm. <br />
[3] Fedesoriano. (September 2021). *Heart Failure Prediction Dataset*. Retrieved [20 Dec. 2021] from https://www.kaggle.com/fedesoriano/heart-failure-prediction.<br />
[4] “Typical Chest Pain vs. Atypical Chest Pain: Time of Care.” *Time of Care | Online Medicine Notebook, 3 June 2019*, https://www.timeofcare.com/typical-vs-atypical-chest-pain/. <br />
[5] “Left Ventricular Hypertrophy.” *Mayo Clinic*, Mayo Foundation for Medical Education and Research, 25 Nov. 2020, https://www.mayoclinic.org/diseases-conditions/left-ventricular-hypertrophy/symptoms-causes/syc-20374314. <br />
[6] “Angina.” *Mayo Clinic*, Mayo Foundation for Medical Education and Research, 12 June 2020, https://www.mayoclinic.org/diseases-conditions/angina/symptoms-causes/syc-20369373. <br />
[7] “Myocardial Ischemia.” *Mayo Clinic*, Mayo Foundation for Medical Education and Research, 5 May 2021, https://www.mayoclinic.org/diseases-conditions/myocardial-ischemia/symptoms-causes/syc-20375417. 

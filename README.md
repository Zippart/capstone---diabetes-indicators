### Disclaimer: "capstone diabetes" is the only relevant file with code, the rest are outdated

In 2021, 38.4 million Americans, or 11.6% of the population, had diabetes. 2 million Americans have type 1 diabetes, including about 304,000 children and adolescents. The following dataset is from a survey where participants answered various questions about their demographics and health. The end goal of this project was to create predictive models based on the given info.

## 1.	Data
The CDC has this info, but I originally found it from the UC Irvine Machine Learning repository. The data was pre processed with age brackets.

https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators

For more info on CDC Survey Data, please check: https://www.cdc.gov/brfss/annual_data/annual_2014.html

## 2.	Method
I tried three different types of models: random forest, decision tree, and logistic regression.

## 3.	Cleaning
This process was very straight forward. There were no null values and the data was most likely cleaned before I touched it. There was a key given as all the data was numeric. For example, for income, different numbers represented different income brackets.

## 4.	EDA
Most of the participants didn’t have diabetes. Comparing the diabetes status and common health related variables like blood pressure and BMI showed expected correlation. 

<img width="269" alt="image" src="https://github.com/Zippart/capstone---diabetes-indicators/assets/46052439/ca5eb4d6-18ab-4901-be0b-28c84ea2abe5">

<img width="346" alt="image" src="https://github.com/Zippart/capstone---diabetes-indicators/assets/46052439/9dd548fa-6cd3-434b-ad70-15b239ca93a7">


## 5.	Machine Learning

Unfortunately, the models were good at predicting when someone doesn’t have diabetes, but poor at predicting prediabetes or diabetes. Ultimately the random forest had the best results out of the three learning models for predicting positive results with a 63% precision rate and an 11% recall rate. See the model metrics file for more details.

![decision_tree_poster](https://github.com/Zippart/capstone---diabetes-indicators/assets/46052439/050ae21f-824b-40e3-a767-de884f291ddf)

## 6.	Recommendations
The models confirmed that high blood pressure, age, BMI, and high cholesterol were all important factors correlated with prediabetes or diabetes. With this data, other more complicated machine learning models can be updated to include this dataset. Datasets like these can be further proof and evidence for public health initiatives to collaborate with the government for PSAs or for real time clinical decision support for users of the company’s technology.


## 7.	Future Improvements
I want to try out different models and different hyperparameter tuning in the future. I might also increase the scope of the project by finding other diabetes data to predictive model and see how the datasets compare with their features and usefulness in model building. I will soon redo the models removing the general health and mental health features, as those were qualitative in nature instead of quantitative.

## 8.	Credits

Thank you to everyone in the Springboard Slack and my mentor that helped me navigate this project!

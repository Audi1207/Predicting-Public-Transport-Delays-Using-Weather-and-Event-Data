Predicting Public Transport Delays Using Weather and Event Data

## Project Overview
This project aims to analyze and predict public transport delays using external factors such as weather conditions and city events. The goal is to identify patterns that influence delays and build a machine learning model to predict whether a delay will occur.


## Objectives
- Analyze the impact of weather conditions on transport delays  
- Analyze how city events influence delay probability  
- Build a machine learning model to predict delays (0 = no delay, 1 = delay)  


## 📊 Dataset
Source: Kaggle – Public Transport Delays with Weather and Events  

The dataset includes:
- Weather conditions  
- Event types (concert, parade, etc.)  
- Transport types  
- Delay indicator (`delayed`: 0 = no delay, 1 = delay)  


## Exploratory Data Analysis (EDA)

### Event Impact on Delays
- Parade events show the highest delay probability (~76.7%)  
- Concert events also show high delay rates (~73%)  
- Events significantly increase the likelihood of delays  

### General Pattern
- Around 74% of trips experience delays  
- Indicates class imbalance in the dataset  


## 🤖 Machine Learning Models

### Models Used:
- Logistic Regression  
- Logistic Regression (class_weight='balanced')  
- Random Forest  


## Model Evaluation

### Logistic Regression (Baseline)
- High accuracy  
- Strong bias toward predicting delays  

### Logistic Regression (Balanced)
- Improved ability to detect both classes  
- Lower overall accuracy  

### Random Forest
- Accuracy: ~72%  
- Excellent at detecting delays (recall ≈ 97%)  
- Poor performance in detecting non-delay cases  


##  Key Insight
The dataset is imbalanced, which significantly affects model performance.  
There is a trade-off between accuracy and the ability to fairly detect both delay and non-delay cases.


##  Tools & Technologies
- Python  
- Pandas, NumPy  
- Seaborn, Matplotlib  
- Scikit-learn  


##  Conclusion
Event types and external conditions play a significant role in transport delays.  
While machine learning models can predict delays with reasonable accuracy, handling imbalanced data remains a key challenge for improving performance.


##  Repository Structure
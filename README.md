# 🗳️ Voter Behavior Prediction & Text Analytics — Machine Learning + NLP Project

This project includes two major components:  
1. **Predicting voter party choice using ML classification models**  
2. **Text analysis of US presidential inaugural speeches using NLP**

The project demonstrates end-to-end data preprocessing, model building, evaluation, and text mining workflows.

---

## 📌 Problem 1: Voter Party Prediction (Exit Poll Model)

A leading news channel conducted a survey of **1525 voters** with **9 features** including age, economic conditions, political knowledge, and leadership ratings (Blair & Hague).  
Goal: Predict whether a voter will vote for **Conservative** or **Labour**.

### 🔍 Key Steps

#### **1. Exploratory Data Analysis**
- Checked data shape, duplicates, and missing values  
- Removed irrelevant column `Unnamed: 0`  
- Descriptive statistics for all attributes  
- Univariate & bivariate plots  
- Outlier detection using boxplots  
- Pairplots & correlation matrix

#### **2. Data Preparation**
- Encoded categorical variables (`vote`, `gender`)  
- Verified scaling necessity  
- Checked multicollinearity using **VIF**  
- Train–test split: **70% train / 30% test**

---

## 🤖 Models Applied

A total of **7 classification models** were built:

1. Logistic Regression  
2. Linear Discriminant Analysis (LDA)  
3. K-Nearest Neighbors (KNN)  
4. Gaussian Naive Bayes  
5. Random Forest (Bagging)  
6. AdaBoost  
7. Gradient Boosting (Best Model)

### 🏆 Best Performing Model: Gradient Boosting
- **Test Accuracy:** 83.5%  
- **AUC:** 89.93%  
- **High recall, precision, and F1-score**  
- Outperforms all other models in predictive strength  

### 🔑 Insights
- Europe score, Blair rating, and Hague rating are strong predictors  
- Lower economic conditions → Conservative vote  
- High Euroscepticism → Conservative vote  
- Labour voters tend to rate Blair higher and support EU integration  

---

## 📌 Problem 2: NLP Analysis of US Presidential Speeches

Speeches analyzed:
- **Franklin D. Roosevelt (1941)**  
- **John F. Kennedy (1961)**  
- **Richard Nixon (1973)**  

### 🔍 Text Processing Steps
- Lowercasing  
- Removing special characters  
- Tokenization  
- Stopword removal  
- Lemmatization  
- Frequency distribution  
- Word cloud generation  
- Lexical dispersion plots  

### 🧠 Insights
- Roosevelt: Top words — *nation, life, people*  
- Kennedy: Top words — *world, side, power*  
- Nixon: Top words — *America, peace, world*  
- Word clouds confirm speech themes visually

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-Learn  
- Matplotlib, Seaborn  
- NLTK  
- WordCloud  
- Statsmodels  



⭐ If you found this project helpful, consider starring the repository!

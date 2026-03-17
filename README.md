# PRODIGY_DS_01
##  Project Overview

This project focuses on analyzing and visualizing the Titanic dataset to understand patterns in passenger data such as age distribution, gender distribution, survival rates, and class-based insights.

The goal is to use Python libraries to perform exploratory data analysis (EDA) and generate meaningful visualizations.

---

##  Dataset

* Dataset Used: Titanic Dataset
* Source: Kaggle
* File: `train.csv`

---

##  Technologies Used

* Python
* Pandas
* Matplotlib

---

##  Installation & Setup

1. Install required libraries:

```
pip install pandas matplotlib
```

2. Download the dataset from Kaggle and place it in your project folder.

3. Update file path in code:

```
data = pd.read_csv("train.csv")
```

---

##  Features & Visualizations

The project includes the following analyses:

###  Basic Visualizations

* Age Distribution (Histogram)
* Gender Distribution (Bar Chart)
* Survival Count

###  Advanced Visualizations

* Survival by Gender
* Survival by Passenger Class
* Fare Distribution
* Age vs Fare (Scatter Plot)
* Box Plot for Age

###  Additional Insights

* Age Group Analysis
* Survival Rate by Age Group
* Embarked Location Distribution
* Family Size Analysis (SibSp, Parch)
* Correlation Heatmap

---

##  Sample Code

```python
import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("train.csv")

# Age Histogram
plt.hist(data['Age'].dropna())
plt.title("Age Distribution")
plt.show()

# Gender Bar Chart
data['Sex'].value_counts().plot(kind='bar')
plt.title("Gender Distribution")
plt.show()
```

---

##  Key Insights

* Majority of passengers were between ages 20–40
* Female passengers had higher survival rates
* First-class passengers had better survival chances
* Fare varies significantly across passenger classes

---

##  Conclusion

This project demonstrates how data visualization helps in understanding patterns and making data-driven decisions. The Titanic dataset provides a great starting point for beginners in data analysis.

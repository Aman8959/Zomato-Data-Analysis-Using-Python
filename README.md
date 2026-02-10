
# 🍽️ Zomato Data Analysis Using Python

## 📌 Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of Zomato restaurant data using Python.
The goal is to extract meaningful insights such as restaurant types, ratings distribution, online orders, table booking trends, and more.

The analysis is performed using popular Python data analysis and visualization libraries.

## 🎯 Objectives

* Understand restaurant business trends from Zomato dataset
* Analyze ratings and customer preferences
* Explore restaurant types and services
* Identify factors affecting ratings
* Visualize insights using graphs and plots

## 🛠️ Technologies & Libraries Used

* **Python**
* **Pandas** → Data manipulation & analysis
* **NumPy** → Numerical operations
* **Matplotlib** → Data visualization
* **Seaborn** → Statistical visualization
* **Jupyter Notebook** → Development environment
  
## 📂 Dataset Information

* Dataset Name: **Zomato Restaurant Data**
* Format: CSV File
* Contains information such as:

  * Restaurant Name
  * Location
  * Online Order Availability
  * Table Booking
  * Ratings
  * Votes
  * Restaurant Type
  * Approx Cost for Two

## ⚙️ Project Workflow

### 1️⃣ Data Loading

```python
import pandas as pd

dataframe = pd.read_csv("Zomato-data-.csv")
dataframe.head()

### 2️⃣ Data Cleaning

* Converted ratings from string → float
* Handled missing values
* Checked dataset info & null values

Example:

```python
def handleRate(value):
    value = str(value).split('/')
    value = value[0]
    return float(value)

dataframe['rate'] = dataframe['rate'].apply(handleRate)


### 3️⃣ Exploratory Data Analysis

Performed analysis such as:

* Restaurant type distribution
* Online order availability
* Table booking analysis
* Ratings distribution
* Cost vs Rating relationship

### 4️⃣ Data Visualization

Used Seaborn & Matplotlib for plots like:

* Count Plots
* Bar Charts
* Heatmaps
* Histograms

Example:

```python
sns.countplot(x=dataframe['listed_in(type)'])
plt.xlabel("Type of restaurant")
plt.show()

## 📊 Key Insights

* Most common restaurant types identified
* Impact of online ordering on ratings
* Relationship between cost and customer reviews
* Popular service combinations

*(Insights may vary based on dataset)*


## 🚀 How to Run This Project

1. Install required libraries:
   
```bash
pip install pandas numpy matplotlib seaborn

2. Open Jupyter Notebook:

```bash
jupyter notebook

3. Run all cells step-by-step.

## 📁 Project Structure

Zomato-Data-Analysis/
│── Zomato_Data_Analysis_Using_Python.ipynb
│── Zomato-data-.csv
│── README.md
```

## 🔮 Future Improvements

* Build interactive dashboard (Power BI / Tableau)
* Deploy as web app using Streamlit
* Add ML model for rating prediction

---
 👨‍💻 Author
 
Aman kumar yadav
* B.Tech IT Student
* Interested in Data Analysis & AI Projects


# Project1-DES432-EDA-OlympicRecords
Exploratory Data Analysis and Descriptive Statistics of Olympic athlete participation records using the “120 Years of Olympic History: athletes and results” dataset for DES432 Statistics &amp; Data Modeling.

🏅 Olympic Athlete EDA — DES432 Project 1

Exploratory Data Analysis and Descriptive Statistics of Olympic athlete participation records using the “120 Years of Olympic History: Athletes and Results” dataset.

This project was completed for DES432 – Statistics & Data Modeling at Sirindhorn International Institute of Technology (SIIT), Thammasat University.

📌 Project Overview

This project performs data cleaning, exploratory data analysis (EDA), and descriptive statistics on Olympic athlete participation records from 1896–2016.

The analysis focuses on comparing athlete characteristics in two Summer Olympic sports:

🏃 Athletics (Track Events)

🏊 Swimming

These sports were chosen because they:

Have large participation counts

Represent different physical performance demands

Provide meaningful comparison between athlete profiles

The goal is to understand how height, weight, and age differ between sports and how these characteristics relate to medal outcomes.

📂 Dataset

Source: Kaggle – 120 Years of Olympic History: Athletes and Results

Each row represents one athlete in one Olympic event.
Athletes may appear multiple times if they competed in multiple events or years.

Key Variables Used
Variable	Type	Description
Sex	Categorical	Male / Female
Age	Numerical	Years
Height	Continuous	cm
Weight	Continuous	kg
Sport	Categorical	Olympic sport
Event	Categorical	Specific competition
Medal	Categorical	Gold / Silver / Bronze / No Medal
🧹 Data Cleaning

To improve data reliability, the following steps were applied:

Removed duplicate participation records

Standardized text formatting in categorical variables

Re-coded missing medal values as “No Medal”

Converted Age, Height, Weight to numeric format

Removed unrealistic values using valid ranges

Imputed missing values using median by Sport + Sex

After cleaning, the analysis focuses only on:

Athletics (Track Events)

Swimming (Summer Olympics)

📊 Exploratory Data Analysis (EDA)

EDA was performed using histograms, boxplots, bar charts, and scatterplots.

Categorical Exploration

Medal distribution

Sex distribution

Univariate Analysis

Distribution and spread of:

Height

Weight

Age

Bivariate Analysis

Relationships between variables:

Height vs Medal outcome

Height vs Weight

🔎 Key Findings

Most Olympic participants do not win medals, which is expected due to limited medal awards.

Male athletes appear more frequently, though both sexes are well represented.

Swimming athletes are slightly taller and heavier than track athletes.

Height distributions are approximately symmetric.

Weight and age show mild right-skewness and some high-value outliers.

A clear positive relationship between height and weight exists in both sports.

Medal-winning swimmers tend to be slightly taller than non-medalists.

📈 Statistical Summary Choices

Based on distribution shape:

Variable	Summary Measure
Height	Mean + Standard Deviation
Weight	Median + IQR
Age	Median + IQR
Categorical variables	Counts & proportions

These choices ensure summaries match the distribution characteristics observed in EDA.

💻 Repository Structure
Project1-DES432-EDA-OlympicRecords
│
├── Project1_DES432_athlete_events.ipynb   # Main analysis notebook
├── README.md                              # Project documentation
└── Report (PDF)                           # Final project report

🛠 Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn

Google Colab

👩‍🎓 Authors

Nutnapin Chongwimansin — 6622770848

Supitcha Puboonterm — 6622772539

Lalitpatra Kodsup — 6622780730

DES432 Statistics & Data Modeling
SIIT, Thammasat University

📎 Notes

This dataset contains elite Olympic athletes, so results may not represent the general population.

# Project1-DES432-EDA-OlympicRecords

Exploratory Data Analysis (EDA) and Descriptive Statistics on Olympic athlete participation records using the dataset **“120 Years of Olympic History: Athletes and Results.”**

Course: **DES432 – Statistics & Data Modeling (SIIT, Thammasat University)**

---

## 📌 Project Overview
This project cleans and analyzes Olympic athlete participation records (1896–2016) with a focus on two Summer Olympic sports:
- 🏃 **Athletics (Track Events)**
- 🏊 **Swimming**

The goal is to compare athlete physical characteristics (**height, weight, age**) and explore relationships with **medal outcomes** using EDA and descriptive statistics.

---

## 📂 Dataset
Source: Kaggle — *120 Years of Olympic History: Athletes and Results*  
Each row represents **one athlete in one event in one Olympic Games** (athletes may appear multiple times across years/events).

Key variables used:
- **Sex** (categorical)
- **Age** (numerical)
- **Height** (cm, numerical)
- **Weight** (kg, numerical)
- **Sport / Event** (categorical)
- **Medal** (Gold / Silver / Bronze / No Medal)

---

## 🧹 Data Cleaning Summary
Steps applied to improve data quality:
- Removed **duplicate rows**
- Standardized text formatting (trim whitespace)
- Re-coded missing medals as **“No Medal”**
- Converted **Age/Height/Weight** to numeric
- Set unrealistic values to missing (range validation)
- Imputed missing Age/Height/Weight using **median by Sport + Sex** (fallback to overall median)

After cleaning, analysis was restricted to:
- **Summer Olympics**
- **Athletics (Track Events)** and **Swimming**

---

## 📊 Exploratory Data Analysis (EDA)
Visualizations and interpretations include:

### Categorical
- Medal distribution (Track vs Swimming)
- Sex distribution (Track vs Swimming)

### Univariate
- Height distribution (histogram + boxplot)
- Weight distribution (histogram + boxplot)
- Age distribution (histogram + boxplot)

### Bivariate
- Height vs Medal (Track vs Swimming)
- Height vs Weight (Track vs Swimming)

---

## 🔎 Key Findings (High-level)
- Most participation records are **No Medal** (expected due to limited medal awards).
- Swimming athletes are generally **slightly taller and heavier** than track athletes.
- Height is **approximately symmetric**; weight and age show **mild right-skewness**.
- Height and weight have a clear **positive relationship** in both sports.
- Medalists in swimming tend to be **slightly taller** than non-medalists (with overlap across categories).

---

## 📈 Summary Statistics Choice
Based on EDA:
- **Height:** Mean + Standard Deviation  
- **Weight:** Median + IQR  
- **Age:** Median + IQR  
- **Categorical variables:** Counts and proportions

---

## 🗂 Repository Contents
- `Project1_DES432_athlete_events.ipynb` — main notebook (cleaning + EDA + descriptive stats)
- `README.md` — this file
- `DES432_Project1_EDA_Report.pdf` — final report (if uploaded)

> Note: The raw dataset file may be too large for GitHub. If not included, please download it from Kaggle using the link above.

---

# ▶️ How to Run This Project

## Option 1 — Run in Google Colab (Recommended)

### Step 1 — Download Dataset
Download from Kaggle:  
https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results  

Download the file:
```

athlete_events.csv

````

### Step 2 — Open Notebook in Colab
Upload or open the notebook in Google Colab.

### Step 3 — Upload Dataset
In Colab:
1. Open the **Files** panel (left sidebar)
2. Click **Upload**
3. Upload `athlete_events.csv`

### Step 4 — Run All Cells
Click **Runtime → Run all**

The notebook will automatically:
- Clean the dataset  
- Generate plots  
- Compute descriptive statistics  

---

## Option 2 — Run Locally (Python)

### Step 1 — Install Libraries
```bash
pip install pandas numpy matplotlib seaborn jupyter
````

### Step 2 — Download Dataset

Place the dataset file in the project folder:

```
athlete_events.csv
```

### Step 3 — Run Notebook

```bash
jupyter notebook Project1_DES432_athlete_events.ipynb
```

Run all cells from top to bottom.

---

## 📈 Expected Output

Running the notebook will:

* Produce cleaned dataset
* Generate EDA plots
* Print descriptive statistics

```
## 🛠 Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Google Colab

---

## 📎 Note
This dataset represents **elite Olympic athletes**, so findings may not represent the general population.
present the general population.

🚀 SpaceX Falcon 9 Launch Analysis & Prediction

IBM Applied Data Science Capstone Project

📌 Project Overview

SpaceX significantly reduces launch costs by reusing the Falcon 9 first-stage booster.
This project applies end-to-end data science techniques to analyze historical SpaceX launch data and predict whether the first stage will successfully land.

The analysis helps answer:

What factors most influence launch success, and can we reliably predict landing outcomes?

🎯 Objectives

Collect and clean SpaceX launch data

Perform exploratory data analysis (EDA) using visualization and SQL

Analyze geographical launch site factors

Build interactive dashboards for insight exploration

Train and evaluate machine learning classification models

Identify the best-performing predictive model

🗂 Project Structure
IBM-Applied-Data-Science-Capstone/
│
├── data sets
│
├── notebooks
│   ├── 01-data-collection-api.ipynb
│   ├── 02-web-scraping.ipynb
│   ├── 03-data-wrangling.ipynb
│   ├── 04-eda-visualization.ipynb
│   ├── 05-eda-sql.ipynb
│   ├── 06-folium-map.ipynb
│   ├── 07-plotly-dash.ipynb
│   └── 08-ml-prediction.ipynb
│
├── dashboard
│   └── spacex_dash_app.py
│
├── report
│   └── Analysis_Report.pptx
│
└── README.md

📥 Data Collection

SpaceX REST API for structured launch data

Web Scraping for supplementary mission details

Public datasets provided by IBM Skills Network

🧹 Data Wrangling & Feature Engineering

Handled missing values and inconsistencies

Encoded categorical features (orbit, launch site, booster)

Standardized numerical features

Created target variable:

Class = 1 → Successful landing

Class = 0 → Failed landing

📊 Exploratory Data Analysis (EDA)
Visual Analysis

Scatter plots:

Payload vs Launch Site

Payload vs Orbit Type

Flight Number vs Launch Site

Bar charts:

Success rate per orbit

Line chart:

Yearly launch success trend

SQL Analysis

Payload aggregation by customer and booster

Landing outcome frequency analysis

Temporal filtering (yearly & monthly trends)

Subqueries for maximum payload missions

🗺 Geospatial Analysis (Folium)

Mapped all SpaceX launch sites

Visualized success vs failure using colored markers

Distance analysis to:

Coastline

Railways

Highways

Cities

📌 Key Insight:
Launch sites are strategically located near coastlines and transport infrastructure while remaining distant from major cities for safety.

📈 Interactive Dashboard (Plotly Dash)

Features

Launch site dropdown filter

Payload range slider

Pie chart:

Success vs failure by site

Scatter plot:

Payload vs launch outcome (colored by booster version)

🎯 Enables dynamic, user-driven analysis of launch success.

🤖 Predictive Analysis (Classification)
Models Built

Logistic Regression

Support Vector Machine (SVM)

Decision Tree

K-Nearest Neighbors (KNN)

Model Optimization

Feature standardization

Train-test split (80/20)

Hyperparameter tuning using GridSearchCV

Performance evaluation via:

Test accuracy

Confusion matrix

📌 Model Performance
Model	Test Accuracy
Logistic Regression	83.33%
SVM	83.33%
KNN	77.78%
Decision Tree	66.67%

✅ Best Model: Logistic Regression
Chosen for its accuracy, stability, and interpretability.

🏁 Key Findings

Launch success improves with flight experience

KSC LC-39A has the highest reliability

Payloads between 2,000–6,000 kg show higher success rates

LEO and ISS orbits perform better than GTO

Launch success has steadily increased since 2013

🛠 Tools & Technologies

Python (Pandas, NumPy, Matplotlib, Seaborn)

SQL (SQLite)

Folium (Geospatial Visualization)

Plotly Dash (Interactive Dashboard)

Scikit-learn (Machine Learning)

Jupyter Notebook

📎 Project Report

📄 Full presentation and results:
report/Analysis_Report.pptx

🔗 Author

Muhammad Adeel
Data Scientist | Machine Learning Enthusiast

🔗 GitHub:
https://github.com/MuhammadAdeel-DataScientist

📜 Acknowledgments

IBM Skills Network

IBM Applied Data Science Professional Certificate

SpaceX public datasets
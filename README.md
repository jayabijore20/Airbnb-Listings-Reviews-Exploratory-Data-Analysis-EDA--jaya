Airbnb Listings & Reviews – Exploratory Data Analysis (EDA)
---

##📌 Project Overview
This project performs data cleaning, feature engineering, and exploratory data analysis (EDA) on Airbnb listings and reviews datasets.
The analysis aims to uncover pricing patterns, neighborhood trends, review activity, and relationships between host attributes and customer sentiment.

---
##🎯 Objectives
Clean and preprocess Airbnb listings and reviews datasets.

Engineer new features for deeper insights (e.g., price per bedroom, occupancy rate).

Visualize key trends such as price distribution, neighborhood performance, and review activity.

Prepare datasets for advanced analysis or machine learning.

---
##🛠 Tools & Libraries
Python

Pandas – Data manipulation

NumPy – Numerical operations

Matplotlib & Seaborn – Data visualization

---

##📂 Dataset Description
1. Listings.csv
Contains property-level information including:

Listing details (ID, name, location, latitude, longitude)

Host details (host ID, location, response rate, superhost status)

Property info (property type, room type, accommodates, bedrooms)

Price, availability, review scores

2. Reviews.csv
Contains review-level information including:

Listing ID

Review ID

Reviewer ID

Review date

---

##🔗 Data Source
This dataset is publicly available on Kaggle:https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata
Airbnb Listings and Reviews Dataset

cleaned file - both listings and reviews get after running the code file "airbnb eda analysis"

---
##🔍 EDA Steps Performed
Data Import & Initial Inspection

Loaded Listings.csv and Reviews.csv into Pandas DataFrames.

Checked shape, column names, and sample rows.

Data Cleaning

Removed currency symbols from price and converted to numeric.

Dropped columns with more than 50% missing values.

Handled missing values appropriately.

Feature Engineering

price_per_bedroom = price / bedrooms

occupancy_rate = availability_365 / 365

price_category (Budget, Standard, Premium, Luxury) based on price bins.

review_length = number of characters in review comments.

Converted review dates to datetime.

Exploratory Visualizations

Price Distribution – histogram with KDE.

Price by Neighbourhood – boxplot for top neighborhoods.

Price vs Review Rating – scatterplot for price under $1000.

Reviews Over Time – time series trend of reviews.

Data Export

Saved cleaned datasets as:

listings_cleaned.csv

reviews_cleaned.csv

---

##📊 Example Insights
Some neighborhoods show significantly higher price ranges compared to others.

High-rated listings are not always the most expensive.

Review activity trends may indicate seasonal booking patterns.

---

##🚀 How to Run the Project
Clone this repository:

bash
Copy
Edit
git clone https://github.com/yourusername/airbnb-eda.git
cd airbnb-eda
Install dependencies:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn
Place Listings.csv and Reviews.csv in the project folder.

Run the analysis script:

bash
Copy
Edit
python airbnb_eda.py
View generated plots and cleaned CSV files.

---

##📌 Author
Jaya Bijore
Aspiring Data Analyst | Python | SQL | Data Visualization


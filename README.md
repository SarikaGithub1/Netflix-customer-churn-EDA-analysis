# 🎬 Netflix Customer Churn EDA Analysis

This project dives into churn behavior among Netflix-style streaming users, using a rich dataset of 5,000 customers. By examining age, gender, subscription types, device, region, favourite genres, etc. we aim to uncover what keeps customers hooked — and what drives them away.

---

## 🎯 Objective

- Clean and prepare the raw dataset for meaningful analysis
- Explore churn trends across multiple customer dimensions
- Create insightful visualizations to support strategic decisions

---

## 📦 Dataset Columns

| Column Name                | Description                                 |
|---------------------------|---------------------------------------------|
| `customer_id`             | Unique identifier for each customer         |
| `age`                     | Age of the customer                         |
| `gender`                  | Gender identity                             |
| `subscription_type`       | Type of streaming subscription (e.g., Basic, Standard, Premium) |
| `watch_hours`             | Total streaming hours per month             |
| `last_login_days`         | Days since last login                       |
| `region`                  | User's geographic location                  |
| `device`                  | Preferred viewing device (e.g., TV, Mobile, Desktop, etc) |
| `monthly_fee`             | Monthly fee for subscription                |
| `churned`                 | Whether the customer left (Yes/No)          |
| `payment_method`          | Chosen method of payment                    |
| `number_of_profiles`      | Number of user profiles on account          |
| `avg_watch_time_per_day`  | Average daily viewing time                  |
| `favorite_genre`          | Most watched content genre                  |

---
## 📁 Project Structure

```text
Netflix-customer-churn-EDA-analysis/
├── Data/
│   └── netflix_customer_churn.csv         # Raw dataset containing user information
├── notebooks/
│   └── netflix_customer_churn.ipynb       # Jupyter Notebook with all EDA steps
├── visuals/ │
│   └── visualizations Folder              # Saved visualizations and plots
│       └── Age dist by churn.png
│       └── gender dist by churn.png
│       └── last login days by churn.png
│       └── most favourite genre.png
│       └── most used payment method.png
│       └── region dist by churn.png
│       └── subscription type by churn.png
├── README.md                              # Project documentation
```

## 🔍 Exploratory Data Analysis Steps

1. ✅ Imported libraries and CSV data into a Pandas DataFrame  
2. 🧹 Dropped irrelevant columns and merged two into one  
3. 📋 Summarized DataFrame using `df.info()` and `df.describe()`  
4. 🧼 Removed duplicates and checked for null values  
5. ✂️ Applied lambda functions to string-strip object-type columns  
6. 🔢 Used `df.nunique()` to count unique values  
7. 🔍 Explored `column.unique()` for key categorical features  
8. 📊 Created histplots for:
    - Age distribution by churn
    - Last login days by churn  
9. 📊 Created countplots for:
    - Gender distribution by churn
    - Region distribution by churn
    - Subscription type distribution
    - Payment methods
    - Favorite genres

---

## 🌟 Key Insights

- Churn is more frequent among customers aged around 20 or 45.
- Users inactive for over 30 days are highly likely to churn.
- Majority of users are female, and they also show the highest churn rate.
- Europe and South America exhibit the highest churn volumes.
- Customers with **Basic** subscriptions tend to churn more than those on higher tiers.
- Debit cards are the most used, followed by PayPal.
- Drama is the most favored genre, closely followed by Documentary.



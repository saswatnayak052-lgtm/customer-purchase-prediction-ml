# 🛒 E-Commerce Customer Behavior Analysis & Purchase Prediction

An end-to-end data analytics and machine learning project using Python and Power BI to analyze customer clickstream paths, uncover shopping patterns, and predict user purchase behavior.

---

## 📊 Business Intelligence & Key Data Insights

The deep data analysis and interactive Power BI dashboard revealed several critical business insights:

* **📱 Mobile-First Consumer Base:** Analytics show that the highest volume of user traffic and peak session durations originate from mobile devices. Optimizing the mobile user experience is the highest strategic priority for the business.
* **📈 High-Intent Engagement Curve:** A strong positive correlation exists between our engineered feature (`engagement_score = time_on_site × pages_viewed`) and conversion behavior. Once a specific engagement threshold is crossed, the probability of conversion accelerates up to 99%.
* **🔁 Effective Customer Retention:** The store's conversion rate is heavily driven by returning users and customers with high cart counts. The dashboard shows approximately 4.2K returning users converting directly into the purchase funnel, validating the success of customer loyalty metrics.

---

## 📌 Project Objectives

The primary goal of this project is to analyze e-commerce metrics and establish a predictive framework through:
1. **Data Cleaning:** Imputing missing numerical/categorical values and handling duplicate rows.
2. **Feature Engineering:** Creating a domain-specific custom metric (`engagement_score`) to map user interaction depth.
3. **Exploratory Data Analysis (EDA):** Mapping behavioral trends across session times, bounce rates, and device preferences.
4. **Predictive Modeling:** Training Machine Learning models to accurately classify and predict final customer purchase status.

---

## 🛠️ Technologies Used

* **Programming Language:** Python
* **Data Preprocessing & Visualization:** Pandas, Matplotlib, Seaborn
* **Machine Learning Framework:** Scikit-Learn
* **Business Intelligence (BI):** Power BI Desktop
* **Development Environment:** Google Colab / Jupyter Notebook

---

## 🔍 Dataset Features & Architecture

The machine learning models process the following customer tracking features:

* **Age:** Age of the customer.
* **Gender:** Female / Male.
* **Device Type:** Mobile / Desktop / Tablet.
* **Time on Site:** Total time spent browsing in minutes.
* **Pages Viewed:** Number of pages opened during the session.
* **Previous Purchases:** Historical order count by the user.
* **Cart Items:** Count of products left/added in the cart.
* **Returning User:** Binary flag (0/1) for past store visits.
* **Engagement Score:** Engineered feature combining duration and page depth (`time_on_site` × `pages_viewed`).
* **Purchase Status (Target):** Final conversion outcome (0 = No Purchase, 1 = Purchased).

---

## 🤖 Machine Learning Pipeline & Results

The preprocessing pipeline handles missing values using median imputation for numerical attributes and mode imputation for categorical predictors. To eliminate data leakage and ensure stable validation, the processed data is partitioned into an **80% training** and **20% testing** validation split.

The classification performance of both deployed models is detailed below:
* **Logistic Regression Model:** Achieved ~99% validation accuracy (configured with `max_iter=1000`).
* **Random Forest Classifier:** Achieved ~99% validation accuracy (configured with `n_estimators=50`, `max_depth=5`).

---

## 📁 Files Included

* `ecommerce_user_behavior_8000.csv` – Raw Kaggle user tracking dataset.
* `cleaned_data.csv` – Post-imputation dataset used for Power BI visualization.
* `project_notebook.ipynb` – End-to-end Python pipeline script for cleaning, engineering, and ML modeling.

---

## 🚀 Future Improvements

* Wrapping the predictive Random Forest model with a FastAPI application to create a real-time prediction microservice.
* Integrating real-time streaming data queues directly with the dashboard architecture for dynamic reporting.
 ## 📷 Screen Short
 <img src="https://github.com/saswatnayak052-lgtm/customer-purchase-prediction-ml/blob/main/Screenshot%20(116).png" width="800" alt="Dashboard Preview">
 

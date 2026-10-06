# 🛒 E-Commerce Customer Behavior Analysis & Purchase Prediction

An end-to-end data analytics and machine learning project using Python and Power BI to analyze customer clickstream paths, uncover shopping patterns, and predict user purchase behavior.

---

## 📊 Business Intelligence & Key Data Insights

Project ke data analysis aur Power BI dashboard se niche diye gaye important business insights nikal kar aaye hain:

* **📱 Mobile-First Consumer Base:** Analytics se pata chala hai ki sabse zyada traffic aur peak session durations Mobile devices se aa rahe hain. Business ke liye mobile user experience ko optimize karna sabse badi priority hai.
* **📈 High-Intent Engagement Curve:** Hamaare engineered feature (`engagement_score = time_on_site × pages_viewed`) aur purchase behaviors ke beech ek strong positive correlation hai. Ek specific engagement score cross karte hi conversion ka chance 99% tak badh jata hai.
* **🔁 Customer Retention Success:** Store ka conversion rate returning users aur high cart items waale users se driven hai. Dashboard ke mutaabik, lagbhag 4.2K returning users directly purchase funnel mein convert ho rahe hain, jo customer loyalty ko prove karta hai.

---

## 📌 Project Objectives

Is project ka main goal e-commerce metrics ko analyze karna aur ek predictive framework banana hai:
1. **Data Cleaning:** Missing numerical/categorical values ko treat karna aur duplicate rows ko handle karna.
2. **Feature Engineering:** Domain-specific custom metric (`engagement_score`) create karna jo user interaction depth ko track kare.
3. **Exploratory Data Analysis (EDA):** Session times, bounce rates, aur device preferences ke patterns ko map karna.
4. **Predictive Modeling:** Machine Learning models train karna taaki customer ka final conversion status accurately predict kiya ja sake.

---

## 🛠️ Technologies Used

* **Programming Language:** Python
* **Data Preprocessing & Visualization:** Pandas, Matplotlib, Seaborn
* **Machine Learning Framework:** Scikit-Learn
* **Business Intelligence (BI):** Power BI Desktop
* **Development Environment:** Google Colab / Jupyter Notebook

---

## 🔍 Dataset Features & Architecture

Machine learning models processed the following features from the clickstream dataset:

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

Data preprocessing pipeline mein missing values ko handle karne ke liye numerical columns par median imputation aur categorical columns par mode imputation ka use kiya gaya hai. Data leakages se bachne ke liye preprocess kiye gaye data ko **80% training** aur **20% testing** splits mein partition kiya gaya.

Dono trained models ka classification accuracy performance niche diya gaya hai:
* **Logistic Regression Model:** Achieved ~99% validation accuracy (max_iter=1000).
* **Random Forest Classifier:** Achieved ~99% validation accuracy (n_estimators=50, max_depth=5).

---

## 📁 Files Included

* `ecommerce_user_behavior_8000.csv` – Raw Kaggle user tracking dataset.
* `cleaned_data.csv` – Post-imputation dataset used for Power BI visualization.
* `project_notebook.ipynb` – End-to-end Python pipeline script for cleaning, engineering, and ML modeling.

---

## 🚀 Future Improvements

* Predictive Random Forest model ko FastAPI application ke sath wrap karke real-time prediction microservice banana.

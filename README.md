# Customer Segmentation with Explainable AI (LIME)

This project performs **customer segmentation** on a retail dataset using **KMeans clustering**, and explains cluster assignments using a **Random Forest surrogate classifier** and **LIME**. It is designed to showcase **unsupervised learning, feature engineering, and explainable AI techniques**.

---

## **Project Overview**

Understanding customers is key for businesses. This project segments customers based on purchase behavior, demographics, and preferences, then interprets **why a customer belongs to a particular segment** using LIME.

**Dataset Features:**
- Customer demographics: Age, Gender, Location
- Purchase behavior: Item Purchased, Category, Purchase Amount, Frequency, Previous Purchases
- Other features: Size, Color, Season, Payment Method, Subscription Status, Discount Applied, Review Rating

---

## **Pipeline Steps**

1. **Data Preprocessing**
   - Handle numeric and categorical columns
   - Convert object columns to numeric
   - Encode categorical features using LabelEncoder
   - Scale numeric features with StandardScaler

2. **Clustering**
   - Use KMeans to identify customer segments
   - Visualize clusters using PCA

3. **Surrogate Classifier**
   - Train a Random Forest classifier to predict cluster labels
   - Enables probability-based explanations for LIME

4. **Explainable AI (LIME)**
   - Explain individual customer cluster assignments
   - Identify top features influencing cluster membership

5. **Cluster Analysis**
   - Cluster sizes
   - Average numeric and categorical features
   - Most common purchased items per cluster

---

## **Visualizations**
- PCA scatter plot of clusters
- LIME explanations showing feature importance per customer

---

## **Libraries Used**
- pandas, numpy
- scikit-learn (KMeans, RandomForestClassifier, PCA, preprocessing)
- seaborn, matplotlib
- lime

---

## **Key Takeaways**
- Segmented 3,900 customers into 4 meaningful clusters
- Explained cluster assignments for individual customers
- Identified key features influencing customer behavior
- Demonstrates **integration of unsupervised ML and explainable AI**

---

## **How to Run**
1. Clone this repository
2. Install dependencies:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib lime

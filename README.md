# Data-analyst-portfolio
Site web personnel d’un statisticien et data analyst mettant en valeur ses compétences, projets, analyses de données et visualisations. Une vitrine professionnelle pour présenter son parcours, son expertise en data science et ses services en analyse statistique. 
# Customer Segmentation Analysis – Wholesale Customers

📌 Project Overview

This project performs a customer segmentation analysis using the Wholesale Customers Dataset (Kaggle). The objective is to understand customer purchasing behavior and identify high-consumption segments to support inventory optimization and stock management.

The analysis is implemented in Python and relies on unsupervised learning (K-means clustering).

 🎯 Objectives

* Segment customers based on their purchasing behavior
* Identify high-value / high-consumption customer groups
* Provide analytical insights to support inventory optimization decisions

 📂 Dataset

Source: Kaggle – Wholesale Customers Dataset

The original dataset contains 8 variables:

* 6 numerical variables representing annual spending in product categories:

  * Fresh
  * Milk
  * Grocery
  * Frozen
  * Detergents_Paper
  * Delicassen
* 2 categorical variables:

  * Channel
  * Region

For this analysis, the two categorical variables (Channel and Region) were removed in order to apply PCA and K-means clustering, which require numerical inputs.

Each row corresponds to a customer.

🛠️ Methodology

1. Descriptive Analysis to understand data distribution and variability
2. Data Standardization using `StandardScaler`
3. K-means Clustering
4. applied to standardized data
5. Model Selection:

   * Elbow Method (Inertia)
   * Silhouette Score
 📊 Descriptive Insights

* Strong variability across all product categories
* Right-skewed distributions driven by high-consumption customers
* Significant differences between minimum, median, and maximum values

These observations justify the use of clustering techniques.

 🔍 Clustering Results
 Optimal Number of Clusters

k = 3 selected based on the Elbow Method
 Silhouette Score = 0.458, indicating a moderate but meaningful cluster structure

# Customer Segments Interpretation

# 🔹 Cluster 0 – Moderate Consumers

* Balanced and moderate spending across all categories
* Represents stable and predictable demand

# 🔹 Cluster 1 – Fresh & Frozen Intensive Consumers

* Very high consumption of Fresh and Frozen products
* High spending on Delicassen
* Likely restaurants, hotels, or catering services

➡️ Strategic segment for managing perishable inventory

# 🔹 Cluster 2 – Grocery & Detergents Intensive Consumers

* Extremely high consumption of Milk, Grocery, and Detergents_Paper
* High-volume, fast-rotation demand
* Likely retailers or resellers

➡️ Critical segment for **bulk stock planning and logistics**

## Objective Achievement Assessment

| Objective                                 | Status                |
| ----------------------------------------- | --------------------- |
| Customer segmentation                     | ✅ Achieved            |
| Identification of high-consumption groups | ✅ Achieved            |
| Inventory optimization support            | ⚠️ Partially achieved |

The analysis provides a strong analytical basis for inventory decisions, though full operational optimization would require temporal and cost-related data.

 💡 Business Implications

* Segment-based inventory strategies
* Prioritization of high-consumption customer groups
* Reduced risk of stockouts and overstocking



 🚀 Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib / Seaborn



 📌 Conclusion

The project demonstrates how unsupervised learning can effectively reveal distinct customer purchasing behaviors in the wholesale sector. The identified segments provide actionable insights for inventory management and strategic decision-making

📬 *Feel free to fork, star, or contribute to this project.*


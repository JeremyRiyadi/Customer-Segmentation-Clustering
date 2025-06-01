## 📁 Dataset Overview

This dataset contains information related to **customer transactions** from a retail company. The data includes customer demographic information, purchasing behavior, and details of the products purchased. This dataset is used for **unsupervised learning**, specifically **customer segmentation (clustering)**

### 📌 Main Feature:

* `Customer ID`, `Gender`, `Birth Date`, `Location`
* `Item Purchased`, `Category`, `Purchase Amount (USD)`
* `Size`, `Color`, `Season`, `Review Rating`
* `Subscription Status`, `Shipping Type`, `Discount Applied`, `Promo Code Used`
* `Previous Purchases`, `Preferred Payment Method`, `Frequency of Purchases`

---

## 🧹 Data Preprocessing

The preprocessing steps taken include:

* Converting `Birth Date` to `Age`
* Encoding categorical features using One-Hot Encoding
* Handling missing values
* Normalizing numeric data (MinMaxScaler)
* Selecting relevant features for clustering

---

## 📊 Exploratory Data Analysis (EDA)

Some of the analyses and visualizations performed:

* Customer age distribution
* Customer gender comparison
* Purchase Amount distribution
* Correlation between numeric features
* Analysis of the relationship between subscription status and purchase frequency

---

## 🔍 Clustering Approach

### Method :

* **K-Means Clustering**
  
### Determining the number of clusters using :

* **Elbow Method**
* **Silhouette Score**

### Results:

* Optimal cluster found at `k = X` (depending on silhouette or elbow results)
* Visualization of clustering results with PCA (2D)
* Analysis of the characteristics of each cluster (for example: cluster A contains young customers with high purchases, cluster B contains passive customers with few transactions, etc.)

---

## 📈 Evaluation

* Visualization of inertia and silhouette score shows that the cluster division is quite good.
* Interpretation of each cluster based on:

* Age
* Shopping value
* Purchase frequency
* Payment method and subscription preferences

---

## 📌 Conclusion

* Clustering successfully divides customers into several different segments based on behavior and demographics
* Segmentation results can be used by the marketing team for more targeted marketing strategies (e.g. targeting specifically for customers with high frequency or low purchase value but potential)

---

## 📁 File

* `2A.tsv` - Customer transaction dataset
* `clustering.ipynb` - Analysis and clustering notebook
* `README.md` - This documentation

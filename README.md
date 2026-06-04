# 🛒 SmartCart Customer Segmentation System

_Identifying customer personas to enable personalized marketing, customer retention, and data-driven business decisions using Unsupervised Machine Learning and Python._

---

## 📖 Table of Contents

- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#clustering-techniques">Clustering Techniques</a>
- <a href="#results--business-impact">Results & Business Impact</a>
- <a href="#how-to-run-the-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#author">Author & Contact</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project develops an Intelligent Customer Segmentation System for SmartCart using Unsupervised Machine Learning. The goal is to identify distinct customer groups based on purchasing behavior, demographics, and engagement patterns to improve marketing effectiveness and customer retention.

---

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

SmartCart relied on generic marketing strategies for all customers, resulting in:

- Inefficient marketing campaigns
- Poor customer targeting
- Low customer retention
- Difficulty identifying high-value customers
- Suboptimal marketing ROI

This project aims to solve these challenges through customer segmentation and behavioral analysis.

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

Dataset Information:

- 📊 2,240 Customer Records
- 📋 22 Features

Key Features

- Income
- Age
- Marital Status
- Customer Tenure
- Total Spending
- Number of Deals Purchases
- Web Purchases
- Store Purchases
- Website Visits
- Campaign Response
- Complaints

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)
- K-Means Clustering
- Agglomerative Clustering
- PCA (Principal Component Analysis)
- Jupyter Notebook
- GitHub

---

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
Kmeans-Agglomerative-Clustering-Customer-Segmentation/
│
├── README.md
├── .gitignore
├── requirements.txt
├── Customer_Segmentation_Report.pdf
│
├── Data/
│   ├── Customer Personality Analysis.csv
│   └── Problem Statement.pdf
│
├── Notebook/                # Jupyter Notebook
│   └── Customer Segmentation.ipynb
```

---

<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

- Imputed missing values in the Income feature using median imputation
- Created business-driven features including Age, Customer Tenure, Total Spending, and Total Children
- Consolidated Education levels into Undergraduate, Graduate, and Postgraduate categories
- Transformed Marital Status into customer living arrangements (Partner / Alone)
- Removed redundant columns after feature engineering to improve model efficiency
- Identified and removed outliers (Age > 90 and Income > 600,000), reducing records from 2,240 to 2,236
- Performed One-Hot Encoding on categorical features (Education and Living_with)
- Applied StandardScaler to normalize features before clustering analysis
- Reduced dimensionality using PCA (3 Components) for visualization and cluster interpretation


Result:

- Records before outlier treatment: **2,240**
- Records after outlier treatment: **2,236**

---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>


Key findings from EDA:

- Income shows strong positive correlation with Total Spending (**0.79**)
- Catalog Purchases strongly influence Total Spending (**0.78**)
- Website Visits negatively correlate with Income (**-0.65**)
- Customers with higher spending tend to respond better to campaigns

---

<h2><a class="anchor" id="clustering-techniques"></a>Clustering Techniques</h2>

- K-Means Clustering:
Used Elbow Method and Silhouette Score to determine optimal cluster count (**K = 4**)
- Agglomerative Clustering:
Performed hierarchical clustering using Ward Linkage.
- Final Selection:
Agglomerative Clustering achieved better cluster separation and more meaningful customer segmentation.

---

<h2><a class="anchor" id="results--business-impact"></a>Results & Business Impact</h2>

1. **Optimal Clusters:** Elbow Method identified **K = 4** as the optimal number of customer segments.

2. **Best Clustering Model:** Agglomerative Clustering achieved better cluster separation and customer segmentation compared to K-Means Clustering.

3. **Customer Segmentation:** Successfully segmented **2,240 customers** into **4 distinct customer personas** based on purchasing behavior, demographics, and engagement patterns.

4. **Customer Profile Discovery:** Clusters **0 & 2** were characterized by lower spending behavior and higher digital engagement, while Clusters **1 & 3** exhibited higher income, stronger purchasing power, and better campaign response rates.

5. **Business Impact:** Customer segmentation revealed significant differences in customer behavior, enabling more effective customer targeting, improved retention strategies, optimized marketing spend, and increased campaign ROI.

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:

```bash
git clone https://github.com/Tisha34/Kmeans-Agglomerative-Clustering-Customer-Segmentation.git
```

2. Load the CSV file and import into jupyter notebook

3. Open and run notebook:
   - 'Notebook\Customer_Segmentation_System.ipynb'

---

<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

- Offer discount coupons and bundle promotions to Family Shoppers to improve engagement and purchase frequency.

- Introduce loyalty programs and premium memberships for Loyal Premium Customers to maximize retention and lifetime value.

- Deploy retargeting campaigns and personalized product recommendations for Digital Browsers to increase conversion rates.

- Provide VIP services and exclusive offers to High ROI Customers to strengthen loyalty and maximize revenue generation.

---

<h2><a class="anchor" id="author"></a>Author & Contact</h2>

**Tisha Gandhi**

Data Analyst | Machine Learning Enthusiast |

📧 Email: gandhitishav@gmail.com

🔗 [LinkedIn](www.linkedin.com/in/tisha-gandhi-994b4a24a)

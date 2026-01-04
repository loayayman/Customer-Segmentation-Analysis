# Customer Segmentation & Marketing Strategy Analysis 

## Project Overview
This project performs an **Unsupervised Learning** analysis on a marketing campaign dataset to segment customers into distinct personas using **PCA** and **Agglomerative Clustering**. 

The main objective is to derive actionable marketing strategies for each segment to improve campaign efficiency, customer retention, and revenue.

## Technologies & Libraries
* **Language:** Python 3.x
* **Data Manipulation:** `pandas`, `numpy`, `datetime`
* **Visualization:** `matplotlib`, `seaborn`, `yellowbrick`
* **Machine Learning:** `scikit-learn`
    * Preprocessing: `LabelEncoder`, `StandardScaler`
    * Decomposition: `PCA`
    * Clustering: `AgglomerativeClustering`

## Dataset
* **Source:** `marketing_campaign.csv`
* **Size:** 2,240 records, 29 features.
* **Key Attributes:** Demographics, Household composition, Spending habits, and Campaign engagement.

## Methodology

1.  **Data Cleaning:** Handled missing values in `Income`, removed outliers (Age > 90, Income > 600k), and parsed dates.
2.  **Feature Engineering:** Created new features like `Age`, `Spent` (Total Spend), `Family_Size`, `Is_Parent`, and `Customer_For` (Loyalty duration).
3.  **Preprocessing:** Applied `LabelEncoder` for categorical data and `StandardScaler` for normalization.
4.  **Dimensionality Reduction:** Used **PCA (Principal Component Analysis)** to reduce dimensions to 3 components for better clustering and visualization.
5.  **Clustering:** * Determined optimal clusters ($k=4$) using the **Elbow Method**.
    * Applied **Agglomerative Clustering**.

## Cluster Profiling & Insights

The analysis identified **4 distinct customer segments**:

### Cluster 0: The Established Family
* **Profile:** Older parents, typically with teenagers. Medium family size (2–4).
* **Behavior:** Seek convenience and value.
* **Strategy:** Offer family value packs, multi-buy discounts, and ready-made meal kits.

### Cluster 1: The New Parents
* **Profile:** Younger demographic, small families (usually one young child).
* **Behavior:** Child-focused purchases, health-conscious.
* **Strategy:** Promote fresh produce and organic baby products via social media and app-based coupons.

### Cluster 2: The Elite Spenders
* **Profile:** High income, no children (singles/couples).
* **Behavior:** Highest spenders on wine and meat.
* **Strategy:** Focus on premium/gourmet items, exclusivity, and quality.

### Cluster 3: The Budget Large Family
* **Profile:** Older parents, large families (up to 5), lower income.
* **Behavior:** Price-sensitive, deal seekers.
* **Strategy:** Promote private-label brands, bulk packaging, and aggressive loyalty rewards.

## Visualizations

### 3D Cluster Visualization (PCA)
<img src="https://github.com/user-attachments/assets/29c6a05b-11e3-4504-9950-5825c8e4dbfa" alt="3D Clusters" width="700"/>

### Elbow Method
<img src="https://github.com/user-attachments/assets/71de50e8-e810-4342-8655-55e721c81449" alt="Elbow Method" width="700"/>

### Income vs. Spending per Cluster
<img src="https://github.com/user-attachments/assets/5dcb4f19-40fc-44b0-8021-d68c5e9c9518" alt="Income vs Spending" width="700"/>

### Promotion Acceptance
<img src="https://github.com/user-attachments/assets/2feab4e7-d2df-4c84-96a4-ce6a417fdb98" alt="Promotion Acceptance" width="700"/>

## How to Run

1.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick
    ```
2.  **Run the script:**
    ```bash
    python Unsupervised_Learning_Project.ipynb
    ```

## Contact
* **Name:** Loay Ayman
* **LinkedIn:** [linkedin.com/in/loayayman](https://linkedin.com/in/loayayman)


## 🏋️ Project: Model Fitness Churn Analysis & Retention Strategy

### Objective

The goal of this project was to develop a **data-driven customer retention strategy** for the Model Fitness gym chain. The analysis aimed to **predict monthly churn probability** and identify the key factors and customer segments driving account cancellation. The final deliverable is a set of **actionable business recommendations** to reduce the overall customer turnover rate.

### Results

The analysis identified the most powerful drivers of churn and segmented the customer base into five distinct groups:

* **Churn Drivers:** The highest risk is linked to **short contract periods (1 month)**, **low attendance** (under 1 class per week), and a **short membership lifetime** (under 3 months).
* **Customer Segmentation (K-Means):**
    * **The Loyalists (Cluster 2):** Showed negligible churn (**2.2%**). This group overwhelmingly uses the longest contracts (12 months) and possesses institutional ties (Partner, Promo\_friends).
    * **High-Risk Dropouts (Cluster 3):** Showed the highest churn rate (**57.3%**). This group uses the shortest contracts, has the lowest attendance, and lacks any social/institutional commitment ties.
* **Predictive Modeling:** The **Random Forest Classifier** provided the best performance metrics (high Recall and Precision) for accurately identifying potential churners one month in advance.

### Tools

| Tool/Library | Purpose |
| :--- | :--- |
| **Python** | Core language for analysis and modeling. |
| **Pandas** | Data cleaning, validation, and feature analysis. |
| **Scikit-learn** | Building and evaluating **Logistic Regression** and **Random Forest** classification models. |
| **Scipy** | **Hierarchical Clustering** (`linkage` and `dendrogram`) for cluster estimation. |
| **Matplotlib & Seaborn** | Visualization of feature distributions, correlation matrix, and cluster analysis (Box Plots). |
| **K-Means** | Customer segmentation for business profiling. |

### Skills Learned

* **Churn Prediction Modeling:** Implementing and comparing binary classification models (RF and LR) for a business problem.
* **Customer Segmentation:** Applying **K-Means clustering** to define distinct user profiles (personas) based on behavioral and contractual data.
* **Metrics Evaluation:** Prioritizing and evaluating model performance using **Precision** (avoiding false positives) and **Recall** (catching all potential churners).
* **Process Improvement:** Translating complex statistical findings (cluster means, correlation) into simple, **actionable marketing and operational steps.**

### Next Steps / Recommendations

The strategy should prioritize reducing the highest risk segment (Cluster 3) by focusing on three principles:

1.  **Incentivize Commitment:** Aggressively promote **long-term contracts (6 or 12 months)** using tiered pricing to move customers out of the high-risk 1-month contract bracket.
2.  **Boost Early Engagement:** Implement an automated intervention (via text/phone) when a customer's frequency drops below **1 visit per week** to re-engage them before they quit.
3.  **Create Social Ties:** Use the **Refer-a-Friend program** as a retention tool, offering existing high-risk customers incentives to refer a friend, thereby introducing a social barrier to prevent sudden abandonment.

---

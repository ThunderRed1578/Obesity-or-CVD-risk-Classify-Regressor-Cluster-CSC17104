<div style="text-align: center;"> 
    <span style="font-size: 40px; font-weight: bold">
        CSC17104 – PROGRAMING FOR DATA SCIENCE
    </span>
</div>

<div style="text-align: center;"> 
    <span style="font-size: 32px; font-weight: bold">
        FINAL PROJECT
    </span>
</div>

<div style="text-align: center;"> 
    <span style="font-size: 24px; font-weight: bold">
        <i>
            README
        </i>
    </span>
</div>

<div style="text-align: right;">
    <span style="font-size: 14px">
        <i>
            Dec 16, 2025
        </i>
    </span>
</div>

| Name | ID |
| --- | --- |
| Lê Võ Nhật Minh | 22120210 |
| Nguyễn Hữu Nghĩa | 22120227 |
| Nguyễn Lê Tấn Phát | 22120262 |

---

<h1 align="center">
    <span style="font-size: 40px; font-weight: bold">
        Table of Content
    </span style>
</h1>

I. [Project Overview](#i)

II. [Dataset](#ii)

III. [Research Questions](#iii)

IV. [Key Findings](#iv)

V. [File Structure](#v)

VI. [How to Run](#vi)

VII. [Dependencies](#vii)

---

<h1 id="i" style="font-weight: bold">I. Project Overview</h1>

This project applies Data Science and Machine Learning techniques to analyze the estimation of obesity levels based on eating habits and physical condition. The study involves rigorous data exploration, statistical hypothesis testing, and the development of both Supervised (XGBoost, Ordinal Classification) and Unsupervised (K-Means Clustering) models.

The goal is to move beyond simple BMI classification to understand the *root causes* of obesity (e.g., "Digital Sedentarism," "Caloric Imbalance") and provide personalized, data-driven lifestyle prescriptions.

---

<h1 id="ii" style="font-weight: bold">II. Dataset</h1>

**Source:** [Obesity or CVD risk (Classify/Regressor/Cluster)](https://www.kaggle.com/datasets/aravindpcoder/obesity-or-cvd-risk-classifyregressorcluster)
**Region:** Mexico, Peru, and Colombia.
**Description:** The dataset contains 2,111 records with 17 attributes, including:
*   **Target:** `NObeyesdad` (7 levels: Insufficient Weight to Obesity Type III).
*   **Physical:** Gender, Age, Height, Weight.
*   **Habits:** High-caloric food (FAVC), Veggie consumption (FCVC), Meal frequency (NCP), Snacking (CAEC), Water intake (CH2O), Physical activity (FAF), Tech usage (TUE), Alcohol (CALC), Transport (MTRANS).

---

<h1 id="iii" style="font-weight: bold">III. Research Questions</h1>

1.  **Calorie Monitoring:** Does the habit of monitoring calories (SCC) mitigate obesity risk in high-calorie diets?
2.  **Predictive Modeling & Prescription:** Can we build a model to accurately predict obesity and use SHAP values to generate personalized lifestyle "prescriptions"?
3.  **Gender Profiling:** Do the primary lifestyle drivers of obesity differ significantly between biological genders?
4.  **Patient Clustering:** Can Unsupervised Learning identify distinct "obesity profiles" (e.g., Genetic vs. Lifestyle-driven)?
5.  **Tech vs. Activity:** Can physical activity neutralize the weight gain risks associated with a digital/sedentary lifestyle?
6.  **Dietary Patterns:** Is there an "optimal" combination of meal frequency and water consumption that minimizes obesity risk?

---

<h1 id="iv" style="font-weight: bold">IV. Key Findings</h1>

*   **The "Calorie Immunity" Effect (Q1):** Calorie monitoring (`SCC`) is a critical protective factor. Among high-risk individuals (poor diet/alcohol), those who monitored calories had a **1.6%** severe obesity rate, compared to **34.1%** for those who did not ($p < 0.001$).
*   **Prescriptive AI (Q2):**
    *   **Safety:** The **Ordinal Classifier** (Frank & Hall decomposition) achieved a low Mean Absolute Error (**0.35**), ensuring the model rarely confuses severe obesity with normal weight.
    *   **Personalization:** SHAP analysis revealed that generic advice fails. For specific severe cases, increasing activity (`FAF`) reduced risk scores by **0.40**, while increasing water (`CH2O`) had negligible impact.
*   **Gender Drivers (Q3):**
    *   **Females:** Driven by *Caloric Imbalance* (Moderate snacking + Very low physical activity).
    *   **Males:** Driven by *Environmental Sedentarism* (High reliance on Automobiles).
*   **The Tech Paradox (Q5):** Contrary to the "Digital Sedentary" myth, Tech Use (`TUE`) is negatively correlated with obesity ($r=-0.30$). The highest risk group is the "Non-Digital Sedentary" demographic (No Tech + No Exercise).
*   **Optimal Habits (Q6):** The standard "3 meals + moderate water" routine is linked to higher risk. The optimal pattern is High Hydration (>2L) + Frequent Meals (NCP=4).
*   **Patient Clusters (Q4):** Identified 4 profiles: *The Veggie-Lovers* (Sedentary but eat healthy), *The Active Tech-Users*, *The Meal Skippers*, and *The Older Generation*.

---

<h1 id="v" style="font-weight: bold">V. File Structure</h1>

```
root
├── 📁 data
│   ├── 📁 processed
│   │   └── 📄 ObesityDataSet_Cleaned.csv
│   └── 📁 raw
│       └── 📄 ObesityDataSet.csv
├── 📁 source
│   ├── 📄 Asking Question.ipynb
│   ├── 📄 Data Collecting.ipynb
│   ├── 📄 Data Exploration.ipynb
│   ├── 📄 Project Summary.ipynb
│   ├── 📄 Question Answering (1, 2).ipynb
│   ├── 📄 Question Answering (3, 4).ipynb
│   ├── 📄 Question Answering (5, 6).ipynb
│   └── 📄 References.ipynb
└── 📝 README.md
```

---

<h1 id="vi" style="font-weight: bold">VI. How to Run</h1>

1. Clone the repository:
2. Install dependencies:
3. Run the notebooks: Start Jupyter Lab or Notebook to view the analysis in order (01 to 06).

---

<h1 id="vii" style="font-weight: bold">VII. Dependencies</h1>

• Python 3.11
• Data Manipulation: pandas, numpy
• Visualization: matplotlib, seaborn
• Machine Learning: scikit-learn (DecisionTree, KMeans, PCA, IsotonicRegression)
• Advanced Modeling: xgboost
• Explainability: shap
• Statistics: scipy
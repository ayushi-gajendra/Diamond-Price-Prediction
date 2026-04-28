# 💎 Diamond Valuation & Market Intelligence Strategy
### *Advanced Statistical Modeling and Linear Regression for Automated Pricing*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Statistics](https://img.shields.io/badge/Method-Hypothesis--Testing-blue)

---

## 🎯 Business Context
In high-volume jewelry retail, manual appraisal of thousands of diamonds creates significant operational bottlenecks. This project develops a **scalable pricing engine** that leverages the "4 Cs" (Carat, Cut, Color, Clarity) to predict market value. 

By integrating **Inferential Statistics** to validate market assumptions and **Machine Learning (Linear Regression)** to automate baseline estimates, this framework reduces manual appraisal cycles and provides a statistically sound "starting price" for expert finalization.

---

## 📂 Phase 1: Statistical Inference & Hypothesis Testing
Before model development, I conducted a deep-dive analysis to ensure our dataset aligned with industry standards and to identify confounding variables that might bias a predictive model.

### 🔍 Key Findings: The "Cut-Carat" Paradox
Initial exploratory analysis showed that "Fair" cut diamonds often carried higher average prices than "Premium" cuts. 
* **The Insight:** Statistical testing confirmed that "Fair" diamonds are cut significantly larger (Mean $\bar{x} = 1.06ct$) to compensate for lower quality, masking the value of the cut.
* **The Solution:** Developed **Price per Carat** as a normalized metric. In this normalized view, the value of "Premium" cuts became statistically evident ($p < 0.001$).



### **Statistical Validation Results**
| Statistical Test | Business Question | p-value | Result |
| :--- | :--- | :--- | :--- |
| **One-Sample Z** | Is our inventory priced above the \$3,750 market avg? | **0.0228** | Significant Elevation |
| **Two-Sample T** | Do Premium cuts command higher raw prices? | **0.2602** | Not Significant (Raw) |
| **Normalized T** | Do Premium cuts command higher price-per-carat? | **< 0.001** | Significant Value |

---

## ⚙️ Phase 2: Predictive Modeling (Multiple Linear Regression)
Leveraging the insights from Phase 1, I built a predictive model to automate the appraisal process.

### **1. Feature Engineering & Pre-processing**
* **Encoding:** Transformed ordinal categorical variables (Cut, Color, Clarity) into numerical formats to capture the grading hierarchy.
* **Multi-collinearity Management:** Analyzed physical dimensions ($x, y, z$) against Carat weight to optimize feature selection and prevent over-fitting.

### **2. Model Evaluation**
* **Algorithm:** Multiple Linear Regression.
* **Error Analysis:** Utilized Mean Absolute Error (MAE) to quantify the average dollar deviation, providing stakeholders with a transparent "confidence margin" for the automated prices.



---

## 📊 Business Impact & ROI
* **Operational Efficiency:** Automated the baseline valuation for the standard inventory, allowing certified gemologists to focus exclusively on high-value or outlier stones.
* **Marketing Intelligence:** Provided data-backed justification for a "Value-at-Size" marketing tier for larger "Fair" cut diamonds and a "Quality-First" tier for "Premium" stones.
* **Supplier Quality Audit:** Conducted a proportion test confirming that incoming shipments meet the 67% "Ideal/Premium" quality threshold, ensuring supply chain consistency.

---

## 🛠️ Technical Stack
* **Languages:** Python (Pandas, NumPy, SciPy)
* **Modeling:** Scikit-Learn (LinearRegression, Train-Test Split)
* **Visualization:** Matplotlib, Seaborn
* **Statistical Logic:** Hypothesis testing (Z-tests, T-tests, Proportion tests)

---

## 👤 Author
**Ayushi Gajendra**
*Data Professional | Bengaluru-based Strategy & Analytics*

* **Focus:** Bridging the gap between technical data science and strategic business growth.

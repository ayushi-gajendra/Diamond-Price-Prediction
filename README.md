# 💎 Diamond Price Analysis & Prediction

A comprehensive statistical analysis and machine learning project for predicting diamond prices using hypothesis testing and linear regression techniques.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Technologies Used](#technologies-used)
- [Analysis Workflow](#analysis-workflow)
- [Results & Insights](#results--insights)
- [Installation & Usage](#installation--usage)
- [Dataset](#dataset)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project showcases advanced statistical analysis and machine learning techniques applied to diamond pricing. As a data analyst working for an online jewelry retailer, the goal is to develop cost-effective models for pricing thousands of diamonds daily based on their characteristics.

### Business Context
Qualified experts aren't always available to determine accurate diamond prices. This project provides data-driven solutions to:
- Estimate mean diamond prices with statistical confidence
- Predict individual diamond prices based on characteristics
- Identify key factors influencing diamond value

## 📁 Project Structure

```
diamond-analysis/
│
├── Diamond-Analysis-I-HypoTesting.ipynb          # Statistical hypothesis testing
├── Diamond-Analysis-II-LinearRegression.ipynb    # Linear regression modeling
├── diamonds.csv                                   # Dataset
└── README.md                                      # Project documentation
```

## ✨ Key Features

### Part I: Hypothesis Testing & Statistical Inference
- **Confidence Interval Analysis**: Calculated 95% confidence interval for mean diamond price
- **Distribution Analysis**: Explored price distribution and skewness patterns
- **Statistical Validation**: Applied Central Limit Theorem for inference on skewed data
- **Business Insights**: Provided stakeholder-ready price estimates

### Part II: Predictive Modeling
- **Simple Linear Regression**: Built single-variable models to understand relationships
- **Multiple Linear Regression**: Developed comprehensive multi-feature models
- **Feature Engineering**: Encoded categorical variables (cut, color, clarity)
- **Model Evaluation**: Used R², residuals, and MAE for performance assessment
- **Multicollinearity Analysis**: Examined feature correlations and interactions

## 🛠️ Technologies Used

- **Python 3.8+**
- **Data Manipulation**: Pandas, NumPy
- **Statistical Analysis**: SciPy, Statsmodels
- **Machine Learning**: Scikit-learn
- **Visualization**: Matplotlib, Seaborn
- **Development Environment**: Jupyter Notebook

## 🔄 Analysis Workflow

### Phase 1: Exploratory Data Analysis
1. Data loading and inspection
2. Descriptive statistics and distribution analysis
3. Correlation analysis and pairplot visualization
4. Feature relationship exploration

### Phase 2: Hypothesis Testing
1. Calculate sample statistics (mean, standard deviation)
2. Compute standard error of the mean (SEM)
3. Construct 95% confidence interval
4. Interpret results for business stakeholders

### Phase 3: Simple Linear Regression
1. Identify dependent variable (Price)
2. Select best independent variable through correlation analysis
3. Train regression model
4. Evaluate model performance (R², coefficients)
5. Generate predictions

### Phase 4: Multiple Linear Regression
1. Incorporate multiple numerical features
2. Encode categorical variables (one-hot encoding)
3. Build comprehensive model
4. Analyze multicollinearity
5. Validate with residual plots and error metrics

### Phase 5: Model Evaluation
1. Compare predicted vs. actual prices
2. Analyze residual distributions
3. Calculate Mean Absolute Error (MAE)
4. Assess R² and adjusted R²
5. Validate model assumptions

## 📊 Results & Insights

### Statistical Findings
- **Mean Diamond Price**: $3,900 (95% CI: [3899.22, 3966.55])
- The price distribution is right-skewed, indicating rare high-value diamonds
- Sampling distribution of mean follows normal distribution (Central Limit Theorem)

### Predictive Model Performance
- **Simple Linear Regression**: Carat weight is the strongest single predictor
- **Multiple Linear Regression**: Combined model explains significant price variance
- **Key Predictors**: Carat, cut quality, color grade, clarity
- **Model Accuracy**: Evaluated using R² score and residual analysis

### Business Insights
- Carat weight has the strongest correlation with price
- Cut quality significantly impacts value after controlling for size
- Color and clarity provide additional predictive power
- Model predictions can serve as baseline for expert price adjustments

## 🚀 Installation & Usage

### Prerequisites
```bash
Python 3.8 or higher
Jupyter Notebook or JupyterLab
```

### Setup
1. Clone the repository
```bash
git clone https://github.com/yourusername/diamond-price-analysis.git
cd diamond-price-analysis
```

2. Create virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels jupyter
```

4. Launch Jupyter Notebook
```bash
jupyter notebook
```

5. Open and run the notebooks in order:
   - `Diamond-Analysis-I-HypoTesting.ipynb`
   - `Diamond-Analysis-II-LinearRegression.ipynb`

## 📈 Dataset

The dataset contains diamond sales data with the following features:

### The Four C's of Diamond Grading
- **Carat**: Weight of the diamond (continuous)
- **Cut**: Quality of the cut (categorical: Ideal, Premium, Very Good, Good, Fair)
- **Color**: Diamond color grade (categorical: D through J)
- **Clarity**: Measure of imperfections (categorical: IF, VVS1, VVS2, VS1, VS2, SI1, SI2, I1)

### Additional Features
- **Price**: Sale price in USD (target variable)
- **Depth**: Total depth percentage
- **Table**: Width of top relative to widest point
- **Dimensions**: x, y, z measurements

## 🎓 Learning Outcomes

This project demonstrates proficiency in:
- Statistical inference and hypothesis testing
- Regression analysis (simple and multiple)
- Feature engineering and encoding
- Model evaluation and validation
- Data visualization and storytelling
- Translating statistical findings to business insights

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- Dataset inspired by the classic diamonds dataset
- Statistical methods based on industry best practices
- Built as part of data analytics portfolio development

---

⭐ If you found this project helpful, please consider giving it a star!

**Keywords**: Data Analysis, Statistical Analysis, Machine Learning, Linear Regression, Hypothesis Testing, Python, Pandas, Scikit-learn, Predictive Modeling, Feature Engineering

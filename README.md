# Modeling Power Plant Energy Output Using Nonlinear Regression and Approximate Bayesian Computation (ABC)

## 📊 Project Overview  
This project implements statistical modeling techniques to predict electrical energy output from a Combined Cycle Power Plant (CCPP) using environmental variables. The analysis employs nonlinear regression models and Approximate Bayesian Computation (ABC) to identify the optimal relationship between environmental conditions and power plant performance.

---

## 🎯 Assignment Details  
- **Module**: 7089 CEM - Introduction to Statistical Methods for Data Science  
- **Institution**: Coventry University
- **Coventry University Student ID Number**: 16544288
- **Student ID**: 250069  
- **Author**: Tek Raj Bhatt

---

## 📈 Dataset Information  
The dataset contains **9,568 observations** collected from a Combined Cycle Power Plant over six years (2006-2011), featuring:

### Input Variables:
- `x1`: Temperature (°C) - Ambient temperature  
- `x3`: Exhaust Vacuum (cm Hg) - Vacuum collected from steam turbine  
- `x4`: Ambient Pressure (millibar) - Atmospheric pressure  
- `x5`: Relative Humidity (%) - Humidity level  

### Output Variable:
- `x2`: Net Hourly Electrical Energy Output (MW)  

---

## 🔬 Tasks Completed  

### **Task 1: Preliminary Data Analysis**  
- Time series plots for input and output variables  
- Distribution analysis with histograms and density plots  
- Correlation analysis and scatter plots  

### **Task 2: Regression Modeling**  
- **2.1**: Parameter estimation for 5 candidate models using least squares  
- **2.2**: Residual Sum of Squares (RSS) calculation  
- **2.3**: Log-likelihood and variance computation  
- **2.4**: AIC and BIC model selection criteria  
- **2.5**: Residual distribution analysis (Q-Q plots)  
- **2.6**: Best model selection  
- **2.7**: Train/test split with 95% confidence intervals  

### **Task 3: Approximate Bayesian Computation (ABC)**  
- Posterior distribution estimation using rejection ABC  
- Joint and marginal posterior visualizations  
- Uncertainty quantification for model parameters  

---

## 🔧 Candidate Models  

The analysis evaluates five nonlinear polynomial regression models:

- **Model 1**: `y = θ₁x₄ + θ₂x₃² + θbias`  
- **Model 2**: `y = θ₁x₄ + θ₂x₃² + θ₃x₅ + θbias`  
- **Model 3**: `y = θ₁x₃ + θ₂x₄ + θ₃x₅³`  
- **Model 4**: `y = θ₁x₄ + θ₂x₃² + θ₃x₅³ + θbias`  
- **Model 5**: `y = θ₁x₄ + θ₂x₁² + θ₃x₃² + θbias`  

---

## 📊 Key Findings  

- Temperature shows the **strongest negative correlation** with power output (**-0.95**)  
- Ambient Pressure demonstrates **positive correlation** with energy generation  
- **Model Selection**: Determined through comprehensive AIC/BIC analysis  
- **Prediction Accuracy**: Achieved low RMSE through optimal model selection  

---

## 🚀 Execution Steps 

### 1. Clone the repository:
```bash
git clone [https://github.com/tekrajbhatta/7089-CEM-Introduction-to-Statistical-Methods-for-Data-Science](https://github.com/tekrajbhatta/ccpp-statistical-modeling/).git
cd ccpp-statistical-modeling
```

### 2. Place dataset:
Add `dataset.csv` to the `data-files/` directory.

### 3. Run the analysis:
- Open the **R Markdown** file in **RStudio**
- Click **"Knit"** to generate the full report
- Alternatively, run code chunks sequentially

## 📁 Repository Structure
```text
├── data-files/
│   ├── dataset.csv           # Original dataset
│   ├── x_250069.csv          # Input variables
│   ├── y_250069.csv          # Output variable
│   └── t_250069.csv          # Time series data
├── tek_raj_bhatt_250069.Rmd  # Main R Markdown file
├── README.md                 # This file
└── .gitignore                # Git ignore file
```

## 🛠️ Technologies Used
- **R** - Statistical computing and analysis  
- **RStudio** - Integrated development environment  
- **R Markdown** - Dynamic document generation  
- **ggplot2** - Data visualization  
- **matlib** - Matrix operations for regression analysis  
- **rsample** - Data splitting and resampling  

---

## 📋 Model Evaluation Metrics
- **RSS** (Residual Sum of Squares)  
- **AIC** (Akaike Information Criterion)  
- **BIC** (Bayesian Information Criterion)  
- **RMSE** (Root Mean Square Error)  
- **MAE** (Mean Absolute Error)  
- **95% Confidence Intervals**  

---

## 🎨 Visualization Features
- Time series plots with custom color palette  
- Distribution histograms with density overlays  
- Correlation scatter plots with regression lines  
- Q-Q plots for residual analysis  
- Joint and marginal posterior distributions  

---

## ⚡ Performance Highlights
- Comprehensive model comparison framework  
- Robust parameter estimation using scaled variables  
- Advanced Bayesian uncertainty quantification  
- Professional visualization with consistent styling  

---

## 📚 Academic Context
This project demonstrates proficiency in:
- **Statistical Modeling**: Nonlinear regression analysis  
- **Model Selection**: Information criteria and cross-validation  
- **Bayesian Methods**: ABC sampling and posterior inference  
- **Data Visualization**: Professional statistical graphics  
- **Reproducible Research**: Well-documented R Markdown workflow  

---

## ⚖️ Academic Integrity
This repository contains coursework submitted for academic assessment. The code is shared for educational purposes and portfolio demonstration. Please respect academic integrity policies if you are currently enrolled in similar courses.

---

## 📞 Contact
- **Name**: Tek Raj Bhatt
- **Student ID**: 250069
- **Coventry University Student ID Number**: 16544288
- **Email**: [250069@softwarica.edu.np](mailto:250069@softwarica.edu.np)

---

⭐ **Star this repository if you find it helpful!**  
📄 **License**: This project is for educational purposes only.

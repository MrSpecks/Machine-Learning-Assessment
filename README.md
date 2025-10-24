# 🏠 Housing Prices: Advanced Exploratory Data Analysis & Feature Engineering

## 📊 Project Overview
This project performs comprehensive Exploratory Data Analysis (EDA) and advanced feature engineering on the Kaggle Housing Prices dataset. The analysis includes data understanding, cleaning, visualization, insights generation, and creation of 50+ engineered features to enhance predictive modeling performance.

**Project Type:** Machine Learning Developer Intern Technical Assessment  
**Domain:** Real Estate / Housing Market Analysis  
**Objective:** Predict house sale prices using advanced data science techniques

## 🗂️ Dataset Information

### Primary Dataset
- **Source:** [Kaggle - House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
- **Location:** `./house-prices-advanced-regression-techniques/train.csv`
- **Size:** 1,460 observations × 80 features
- **Target Variable:** SalePrice (continuous, $34,900 - $755,000)
- **Dataset Type:** Supervised Learning (Regression)

### Additional Files
- `test.csv` - Test dataset for predictions
- `data_description.txt` - Detailed feature descriptions
- `sample_submission.csv` - Submission format

## 🚀 Setup Instructions

### Prerequisites
- **Python:** 3.7 or higher
- **Jupyter:** Notebook or JupyterLab
- **Memory:** Minimum 4GB RAM recommended
- **Storage:** 100MB free space

### Installation Steps
1. **Clone/Download Repository:**
   ```bash
   git clone https://github.com/MrSpecks/Machine-Learning-Assessment.git
   cd Machine-Learning-Assessment
   ```

2. **Install Required Libraries:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Verify Installation:**
   ```bash
   python -c "import pandas, numpy, matplotlib, seaborn; print('✅ All libraries installed successfully!')"
   ```

## ▶️ Execution Instructions

### Main Analysis Notebook
1. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open Main Analysis:**
   - Navigate to `housing_eda_analysis.ipynb`
   - Run all cells sequentially (Cell → Run All)

3. **Expected Runtime:** 5-10 minutes for complete analysis

### Advanced Feature Engineering (Optional)
1. **Open Feature Engineering Notebook:**
   - Navigate to `housing_feature_engineering_kagiso_mfusi.ipynb`
   - Run all cells to create 50+ engineered features

2. **Expected Runtime:** 3-5 minutes for feature creation

### Preliminary Modeling (Optional)
1. **Open Modeling Notebook:**
   - Navigate to `prelim_modelling_kagiso_mfusi.ipynb`
   - Run all cells to train baseline Linear Regression model

2. **Expected Runtime:** 2-3 minutes for model training and evaluation

### Output Files Generated
- `train_cleaned.csv` - Cleaned dataset from main EDA
- `train_engineered.csv` - Enhanced dataset with engineered features
- `baseline_model.pkl` - Trained Linear Regression model
- `preprocessor.pkl` - Data preprocessing pipeline
- Various visualization outputs and analysis reports

## 📁 Project Structure
```
Machine-Learning-Assessment/
├── house-prices-advanced-regression-techniques/
│   ├── train.csv                    # Original training dataset
│   ├── test.csv                     # Test dataset
│   ├── train_cleaned.csv            # Cleaned dataset (EDA output)
│   ├── train_engineered.csv         # Enhanced dataset (Feature Engineering output)
│   ├── data_description.txt         # Feature descriptions
│   └── sample_submission.csv        # Submission format
├── resources/
│   └── ML Intern Assessment.pdf     # Assessment requirements
├── housing_eda_kagiso_mfusi.ipynb       # Main EDA notebook (6 tasks)
├── housing_feature_engineering_kagiso_mfusi.ipynb # Advanced feature engineering notebook
├── prelim_modelling_kagiso_mfusi.ipynb  # Preliminary modeling notebook
├── DATASET_INFO.md                  # Detailed dataset documentation
├── README.md                        # This file
├── requirements.txt                 # Python dependencies
└── .gitignore                      # Git ignore rules
```

## 🎯 Key Findings Summary

### 📈 **Primary Price Drivers**
• **OverallQual** (r=0.79) - Quality dominates pricing over size
• **GrLivArea** (r=0.71) - Living area is the strongest size predictor
• **GarageCars** (r=0.64) - Garage capacity more predictive than bedroom count
• **Location** - Neighborhood creates 3x price variation ($100k-$300k range)

### 🔍 **Surprising Insights**
• **Quality > Size** - OverallQual beats GrLivArea in importance hierarchy
• **All Outliers High-Value** - No low-value outliers, only luxury homes identified
• **Bedroom Count Weak** - BedroomAbvGr only r=0.17 correlation with price
• **Age Plateau Effect** - Depreciation stops after 50 years, historic homes maintain value

### 📊 **Data Quality Excellence**
• **Zero Missing Values** - All 19 features with missing data successfully imputed
• **No Duplicates** - Clean dataset with unique property records
• **Multicollinearity Documented** - High correlations identified for modeling consideration
• **Outliers Retained** - Legitimate luxury properties preserved for analysis

### 🏗️ **Feature Engineering Success**
• **50+ Features Created** - 7 categories: Interactions, Polynomials, Ratios, Binning, Temporal, Domain-Specific, Aggregation
• **High-Impact Features** - QualitySize, TotalQualityScore, PropertyValueIndex show strong predictive power
• **Expected Performance Gain** - R² improvement from 0.85 to 0.90+ with engineered features

### 💼 **Business Insights**
• **Sellers:** Invest in quality renovations over size expansion for maximum ROI
• **Buyers:** Don't overpay for square footage alone - quality and location matter more
• **Agents:** Use neighborhood-specific comparables for accurate pricing
• **Developers:** Location first, then balance quality and size for optimal market positioning

### 🤖 **Modeling Readiness**
• **Clean Dataset** - Ready for immediate modeling with zero preprocessing needed
• **Feature-Rich** - 130+ total features (80 original + 50+ engineered) available
• **Validation Complete** - All features tested for correlation and multicollinearity
• **Expected R² Performance** - 0.85-0.92 range achievable with proper model selection

### 🎯 **Preliminary Modeling Results**
• **Baseline Model** - Linear Regression with R² ≈ 0.80-0.85 (meets expectations)
• **Performance Metrics** - RMSE, MAE, R² calculated and visualized
• **Model Validation** - Train/test split with predicted vs actual analysis
• **Enhancement Potential** - Engineered features show improvement opportunities
• **Next Steps** - Log transformation, regularization, and advanced algorithms recommended

## 📋 Requirements
```
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
scikit-learn>=1.3.0
```

## 👨‍💻 Author Information

**Full Name:** Kagiso Mfusi  
**Email:** Kagisomfusi@outlook.com  
**LinkedIn:** [https://www.linkedin.com/in/kagiso-mfusi-95b329224](https://www.linkedin.com/in/kagiso-mfusi-95b329224)  
**Project Date:** October 2025  
**Assessment:** Machine Learning Developer Intern Technical Assessment

## 📄 License
This project is created for educational and assessment purposes only. The dataset is sourced from Kaggle's public House Prices competition.

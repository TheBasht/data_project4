# **Obesity Risk Analysis and Prediction**

## **Introduction**
This project aims to analyze and predict obesity risk factors using a robust dataset. Leveraging machine learning techniques, including Random Forest optimization, this project uncovers patterns in dietary, physical, and social habits contributing to obesity. The goal is to provide insights and accurate predictions to guide interventions for better health outcomes.

---

# **Project Description**
This project provides:
- **Data Analysis**: Detailed exploration and visualization of obesity-related data using Python (pandas and Spark).
- **Machine Learning**: Random Forest models optimized for performance and accuracy.
- **Interactive Visualizations**: Using Tableau to engage data dashboards and visual summaries.
- **Predictions**: A model predicting obesity risk based on individual habits and characteristics.

---

# **Datasets**

## **Obesity Dataset**
- **File**: [ObesityDataSet.csv](./ObesityDataSet.csv)
- **Source**: The dataset includes comprehensive information on individual habits and health metrics contributing to obesity risk.
- **Format**: CSV
- **Key Fields**: 
  - Age
  - Gender
  - Dietary Patterns
  - Physical Activity Levels
  - BMI Categories

---

# **Methods**

## **1. Data Preprocessing**
- Handled missing values.
- Transformed categorical data into numerical formats for model compatibility.

## **2. Exploratory Data Analysis (EDA)**
- Conducted descriptive statistics and visualizations to uncover trends.
- Used Python libraries such as `matplotlib` and `seaborn`.
- Leveraged Spark for handling and analyzing large-scale data efficiently.

## **3. Machine Learning**
- Implemented a Random Forest algorithm optimized for accuracy.
- Applied hyperparameter tuning to enhance model performance.
- Evaluated the model using the following metrics:
  - **Precision**
  - **Recall**
  - **F1-Score**

## **4. Visualization**
- Developed Tableau dashboards to visually represent obesity risk patterns and key findings.

---

# **Installation Instructions**

## **Prerequisites**
To run this project, you will need:
- **Python**: Version 3.8 or later
- **Apache Spark**: Installed locally or on a cluster
- **Tableau**: Tableau Public or Desktop for visualizations
- **Python Libraries**:
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `pyspark`

## **Steps to Install**

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/obesity-risk-analysis.git
cd obesity-risk-analysis
--

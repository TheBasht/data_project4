

# **Obesity Risk Analysis and Prediction**

## **Introduction**
This project aims to analyze and predict obesity risk factors using a robust dataset. Leveraging machine learning techniques, including Random Forest optimization, this project uncovers patterns in dietary, physical, and social habits contributing to obesity. The goal is to provide insights and accurate predictions to guide interventions for better health outcomes.

---

## **Project Description**
This project provides:
- **Data Analysis**: Detailed exploration and visualization of obesity-related data using Python (pandas and Spark).
- **Machine Learning**: Random Forest models optimized for performance and accuracy.
- **Interactive Visualizations**: Tableau dashboards for engaging visual summaries.
- **Predictions**: A model predicting obesity risk based on individual habits and characteristics.

---

## **Datasets**

### **Obesity Dataset**
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

## **Methods**

### **1. Data Preprocessing**
- Handled missing values.
- Transformed categorical data into numerical formats for model compatibility.

### **2. Exploratory Data Analysis (EDA)**
- Conducted descriptive statistics and visualizations to uncover trends.
- Used Python libraries such as `matplotlib` and `seaborn`.
- Leveraged Spark for handling and analyzing large-scale data efficiently.

### **3. Machine Learning**
- Implemented a Random Forest algorithm optimized for accuracy.
- Applied hyperparameter tuning to enhance model performance.
- Evaluated the model using the following metrics:
  - **Precision**
  - **Recall**
  - **F1-Score**

### **4. Visualization**
- Developed Tableau dashboards to visually represent obesity risk patterns and key findings.

---

## **Installation Instructions**

#### **Install Dependencies**
*  Run the following command to install the required libraries:
```bash
pip install -r requirements.txt
```
### **Set up Spark**
Refer to the [Spark Documentation](https://spark.apache.org/docs/latest/) for setup instructions.

#### Prepare the Dataset
Place ObesityDataSet.csv in the data directory of the project.

#### Run the Notebooks
Open and execute the Jupyter Notebook files:

```bash
jupyter notebook obesity_rf_optimized_01.ipynb
jupyter notebook obesity_rf_optimized_02.ipynb
```

#### View the Results
Review the analysis, EDA, and predictions presented in the notebooks.

### Explore Visualizations
Open the Tableau project files included in the repository to explore interactive dashboards.

### Usage Examples:

Python Workflow Example:

**import pandas as pd**

**from sklearn.ensemble import RandomForestClassifier**

#### 2. Load the dataset
data = pd.read_csv('ObesityDataSet.csv')

#### 3. Preprocess the dataset
X = data.drop('Obesity', axis=1)
y = data['Obesity']

#### 4. Train the Random Forest model
model = RandomForestClassifier()
model.fit(X, y)

#### 5. Predict using a sample input
sample_data = [[23, 'Female', 'Normal diet', 'Regular exercise']]
prediction = model.predict(sample_data)
print(f'Predicted Obesity Risk Category: {prediction[0]}')


###  Languages and Libraries

**Languages**
* Python 3.8
  
**Libraries**
* pandas: v1.3.3
* matplotlib: v3.4.3
* seaborn: v0.11.2
* scikit-learn: v0.24.2
* pyspark: v3.1.2
  
**Visualization Tools**
*Tableau


##  Results
The optimized Random Forest model achieved high precision and recall rates, making it reliable for predicting obesity risk. Tableau dashboards highlight key trends, such as age and dietary patterns significantly influencing obesity risk.
This structure ensures the proper formatting of code blocks without affecting the text below them.



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

## **Dataset**

#### *About the Dataset:*
This dataset estimates obesity levels in individuals from Mexico, Peru, and Colombia, aged 14 to 61, with diverse eating habits and physical conditions. The data was collected via a web-based survey where anonymous users responded to questions about their habits and lifestyle.

**Key Details**
- **File**: [ObesityDataSet.csv](./ObesityDataSet.csv)
  
- **Attributes:**
  
  - **Eating Habits:**
  * Frequent consumption of high-caloric food (FAVC)
  * Frequency of vegetable consumption (FCVC)
  * Number of main meals (NCP)
  * Consumption of food between meals (CAEC)
  * Water consumption (CH20)
  * Alcohol consumption (CALC)
  
  - **Physical Condition:**
  * Caloric consumption monitoring (SCC)
  * Physical activity frequency (FAF)
  * Time spent using technology devices (TUE)
  * Mode of transportation (MTRANS)

- **Demographics:**
   * Gender, Age, Height, and Weight.
     
- **Target Variable:**
  * NObesity, categorizing individuals into obesity levels based on BMI:
  * Underweight: BMI < 18.5
  * Normal Weight: 18.5 ≤ BMI < 24.9
  * Overweight: 25.0 ≤ BMI < 29.9
  * Obesity Type I: 30.0 ≤ BMI < 34.9
  * Obesity Type II: 35.0 ≤ BMI < 39.9
  * Obesity Type III: BMI ≥ 40
  
- **Format:**
  * The dataset is in CSV format, containing:
    * 2111 records
    * 17 attributes
  
- **Applications:**
The data supports multiple analytical tasks:
  * Classification
  * Regression
  * Segmentation
  * Association algorithms

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

### **Prerequisites**
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
  - `jupyter`

## **Steps to Install**

#### **1. Install Dependencies**
Run the following commands to install the required libraries:
```bash
pip install pandas==1.3.3
pip install matplotlib==3.4.3
pip install seaborn==0.11.2
pip install scikit-learn==0.24.2
pip install pyspark==3.1.2
pip install jupyter==1.0.0

```
#### 2. **Set up Spark**
Refer to the [Spark Documentation](https://spark.apache.org/docs/latest/) for setup instructions.


#### 3. Prepare the Dataset
Place ObesityDataSet.csv in the project data directory.

#### 4. Run the Notebooks
Open and execute the Jupyter Notebook files:

```bash
jupyter notebook obesity_rf_optimized_01.ipynb
jupyter notebook obesity_rf_optimized_02.ipynb
```

#### 5. View the Results
Review the analysis, EDA, and predictions presented in the notebooks.

#### 6. Explore Visualizations
Open the Tableau project files included in the repository to explore interactive dashboards.



## Usage Examples:

### Python Workflow Example:

#### 1. Import dependencies
```
import pandas as pd
from sklearn.ensemble import RandomForestClassifier
```

####  2. Load the dataset
```
data = pd.read_csv('ObesityDataSet.csv')
```

#### 3. Preprocess the dataset
```
X = data.drop('Obesity', axis=1)
y = data['Obesity']
```


#### 4. Train the Random Forest model
```
model = RandomForestClassifier()
model.fit(X, y)
```

#### 5. Predict using a sample input
```
sample_data = [[23, 'Female', 'Normal diet', 'Regular exercise']]
prediction = model.predict(sample_data)
print(f'Predicted Obesity Risk Category: {prediction[0]}')
```

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
* Tableau


##  Results

#### **Model Performance**

The Random Forest model demonstrates excellent predictive power, achieving:
```
* Accuracy: ~93%
* Precision: ~92%
* Recall: ~91%
* F1-Score: ~91.5
```
These metrics indicate the model reliably classifies individuals into all obesity categories, with minimal misclassification.

#### **Key Insights:**

Feature Importance:

**Significant predictors of obesity include:**

* Physical Activity Frequency (FAF): Lower activity levels strongly correlate with higher obesity risk.
* Vegetable Consumption (FCVC): Increased vegetable intake reduces obesity likelihood.
* Number of Meals Per Day (NCP): Higher meal frequency is associated with higher obesity levels.

**General Trends:**

* Physical Activity: Active individuals (<1 day per week of activity) are less likely to be obese.
* Dietary Patterns: Poor dietary habits and meal frequency impact obesity risk significantly.

**Optimization Highlights**

* Hyperparameter Tuning: Improved accuracy and model stability by optimizing parameters like the number of trees and tree depth.
* Cross-Validation: Ensured consistent performance across subsets of the data.
  
## **Conclusion**
With its high accuracy and robust design, the model is an effective tool for predicting obesity levels and identifying key behavioral risk factors. These insights are actionable for interventions targeting improved physical activity and healthier dietary patterns.


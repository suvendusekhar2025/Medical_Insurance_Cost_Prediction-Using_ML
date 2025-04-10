# Medical_Insurance_Cost_Prediction-Using_ML:
Here’s a well-structured and detailed project description based on the input:

---

### **Project Title: Medical Insurance Cost Prediction Using Machine Learning**

**Objective:**  
The goal of this project is to develop a machine learning model that accurately predicts medical insurance costs based on various personal and demographic factors.

**Dataset Overview:**  
- The dataset used contains **1,338 records** and **7 features**, stored in a CSV file.  
- The features include: `age`, `sex`, `bmi`, `children`, `smoker`, `region`, and `charges` (target variable).

**Technologies & Libraries Used:**  
- **Python libraries**:  
  - **NumPy** and **Pandas** for data manipulation and preprocessing  
  - **Matplotlib** and **Seaborn** for data visualization  
  - **Scikit-learn (sklearn)** for model selection and evaluation metrics

**Data Preprocessing:**  
- All **categorical (text) values** were converted into **numerical format** using label encoding via the `.replace()` function:  
  - `sex`: female → 1, male → 0  
  - `smoker`: yes → 0, no → 1  
  - `region`: southeast → 0, southwest → 1, northeast → 2, northwest → 3  
- This transformation ensures that the machine learning model can interpret and work with these features effectively.

**Data Visualization:**  
To understand the data distribution and relationships, the following plots were generated:
- **Distribution Plots** (using Seaborn) for:  
  - `bmi`  
  - `age`  
  - `charges`  
- **Count Plots** (using Seaborn/Matplotlib) for:  
  - `sex`  
  - `smoker`  
  - `region`

These visualizations helped in identifying data patterns, skewness, and the impact of categorical variables on the target variable.

**Model Building:**  
- The dataset was split into **training and test sets** using `train_test_split` from `sklearn.model_selection`.
- A **Linear Regression model** was used due to the continuous nature of the target variable (`charges`).

**Model Evaluation:**  
- The model was evaluated using the **R-squared (R²) score**, which measures the proportion of variance explained by the model.
  - **Training R² Score**: **75.15%**
  - **Testing R² Score**: **74.47%**

These scores indicate a good level of generalization and model performance.

---

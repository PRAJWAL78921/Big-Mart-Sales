# Big-Mart-Sales
# Big Mart Sales Prediction

## Project Overview  
This project aims to **predict the sales of products** in various Big Mart outlets based on historical sales data.  
The goal is to build a **predictive model** that can forecast future sales and help the business understand which factors affect product sales, aiding in **inventory management and strategy formulation**.  

---

## Problem Statement  
Big Mart, a retail company, wants to **enhance its sales forecasting capabilities** to manage inventory and improve revenue.  
The objective is to **predict the sales of each product** at different outlets using various **product and outlet features**.  

---

## Dataset  
The dataset used for this project consists of **sales data of 8523 products** across **10 different attributes**, such as:  
- **Item weight**  
- **Item visibility**  
- **Item type**  
- **Outlet-related features**  

---

## Project Steps  

### 1. Data Collection and Preprocessing  
- Loaded the **training and test datasets**.  
- Identified and **handled missing values** using appropriate strategies:  
  - **Mean imputation** for numerical features.  
  - **Mode imputation** for categorical features.  
- Standardized column names and **encoded categorical variables** using label encoding.  

### 2. Exploratory Data Analysis (EDA)  
- Analyzed the **distribution of various features** and their relationships with the target variable **Item_Outlet_Sales**.  
- Visualized **correlations between features** using a heatmap.  
- Used the **Dtale and Klib libraries** to gain deeper insights into the data through interactive visualizations.  

### 3. Feature Engineering  
- Selected **relevant features** based on correlation analysis and business understanding.  
- Performed **label encoding** on categorical variables to convert them into a numerical format suitable for modeling.  

### 4. Data Splitting and Standardization  
- Split the dataset into **training and testing sets**.  
- Applied **standardization** to the features to ensure all variables contribute equally to the model performance.  

### 5. Model Building and Evaluation  
Built and evaluated multiple regression models, including:  
- **Linear Regression**:  
  - R² score: **0.504**  
  - Mean Absolute Error (MAE): **~880.99**  
- **Random Forest Regressor**:  
  - R² score: **0.550**  
  - MAE: **781.78**  

Assessed model performance using metrics such as:  
- **R² score**  
- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**  

### 6. Hyperparameter Tuning  
- Conducted **hyperparameter tuning** on the **Random Forest Regressor** using **GridSearchCV** to optimize performance.  
- The optimal parameters resulted in an **R² score of approximately 0.549**.  

---

## Conclusion  
- The **Random Forest Regressor outperformed** other models, providing a good balance between **bias and variance**.  
- The project demonstrates how **feature engineering** and **model tuning** significantly impact predictive performance.  

---

## Technologies Used  
- **Python** (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib)  
- **Machine Learning Algorithms**: Linear Regression, Random Forest Regressor  
- **Libraries for Data Cleaning & Visualization**: Klib, Dtale  
- **Excel**  

---

## Future Work  
- Experiment with **advanced machine learning algorithms** like **Gradient Boosting or XGBoost** to improve predictive performance.  
- Explore **feature engineering techniques**, such as creating **new features based on domain knowledge** or using interaction terms.  
- Extend the analysis to include **more recent sales data** and additional **product attributes** for a more comprehensive model.  

# Retail Sales Prediction

## Project Overview

This project focuses on building regression models to predict sales for Rossmann retail stores using historical sales data. The goal is to extract actionable insights and build predictive models that help optimize business operations, resource planning, and promotional strategies in a competitive retail environment.

> **Project Type**: Regression (Supervised Learning)  
> **Contributor**: *Anjali Patel*

## Project Summary

Retail sales can be influenced by a variety of dynamic factors such as store location, customer behavior, promotional events, school holidays, and competitor presence. This capstone project explores how these variables affect store-level sales by analyzing two real-world datasets provided by Rossmann.

The project workflow includes:

* Cleaning and merging multiple datasets
* Performing insightful exploratory data analysis (EDA)
* Conducting hypothesis testing to validate assumptions
* Engineering meaningful features
* Building and evaluating regression models (Linear and Lasso)

Ultimately, the aim is to improve sales forecasting accuracy and support data-driven decision-making for retail store management.

## Tools & Technologies Used

* **Language**: Python 3
* **IDE**: Jupyter Notebook
* **Libraries**:

  * `pandas`, `numpy` – for data manipulation
  * `matplotlib`, `seaborn` – for data visualization
  * `scikit-learn` – for machine learning models and metrics
  * `scipy` – for statistical hypothesis testing

## Key Findings

* **Customer Count Correlation**: Strong positive correlation between number of customers and sales.
* **Weekday Trends**: Sales peak on Mondays, likely because many stores are closed on Sundays.
* **Promotion Effectiveness**: Promotional offers significantly boost sales.
* **Holiday Insights**:
  * School holidays contribute to more sales compared to state holidays.
  * Only 17.9% of total sales occur during school holidays.
* **Store Type & Assortment Impact**:
  * Store Type 'a' consistently yields the highest average sales.
  * Assortment type 'b' (extra) drives the best performance.
* **Hypothesis Testing**:
  * A two-sample t-test revealed that stores closer to competitors tend to have significantly different sales patterns (p-value < 0.05).

## Visual Insights

Here are some of the key visualizations used in the notebook:

### 1. **Sales Distribution by Store Type**
![1](https://github.com/user-attachments/assets/2cc274d5-a397-4c48-9bef-449ace0cc68a)

### 2. **Monthly Sales affected by School Holiday**
![2](https://github.com/user-attachments/assets/182fb39e-1075-4b26-ae82-e7eb592bef38)

### 3. **Promotions vs Sales Comparison**
![3](https://github.com/user-attachments/assets/d2217ded-17b0-42de-b6c0-5201cbfd85ff)

### 4. **School vs State Holiday Sales**
![42](https://github.com/user-attachments/assets/c8b950b7-816f-4134-aa7b-f02cb684155b)

![41](https://github.com/user-attachments/assets/dc2c1777-7e93-420e-aa7f-bcb96284b2f6)

### 5. **Correlation Heatmap of Features**
![5](https://github.com/user-attachments/assets/38f674b7-8ee9-41cf-bd47-4d8bc5ae9613)

### 6. **Sales vs Customer Scatter Plot**
![6](https://github.com/user-attachments/assets/f86d9d6d-8fff-4613-8305-c7466e123e3d)

### 7. **Boxplots of Competition Distance Effects**
![7](https://github.com/user-attachments/assets/5c2f8698-603d-4915-9a68-d26137c1b8d7)


## Feature Engineering

* Converted date into useful time-based features like year, month, and day.
* Imputed missing values in competition-related columns.
* Removed outliers in sales and customer data.
* Dropped low-importance or redundant columns (e.g., ‘Customers’, ‘Open’ during preprocessing).
* Encoded categorical features using Label Encoding and One-Hot Encoding as needed.

## Model Building & Evaluation

Two regression models were trained and evaluated:

| Model             | Mean Squared Error (MSE) | R-squared (R²) |
| ----------------- | ------------------------ | -------------- |
| Linear Regression | Moderate                 | Good           |
| Lasso Regression  | **Lower**                | **Higher**     |

**Conclusion**:
The **Lasso Regression model** performed better, offering improved generalization by reducing overfitting and maintaining good feature selection due to its L1 regularization.

## Repository Structure

* **Regression - Retail Sales Prediction** – Main project folder
  * **Regression - Retail Sales Prediction.ipynb** – Jupyter Notebook containing the full analysis
* **LICENSE** – MIT License file
* **README.md** – Documentation explaining the project

## Acknowledgements

* **Dataset Source** - Rossmann Store Sales - Kaggle

##  License

This project is licensed under the **MIT License**. See the `LICENSE` file for more information.

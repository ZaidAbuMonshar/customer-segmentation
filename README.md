# Customer Segmentation Project

# Customer Clustering Notebook

## Overview
This project focuses on clustering customers based on their shopping behavior and demographic information. The goal is to segment customers into distinct groups to help businesses better understand their customer base and tailor marketing strategies accordingly. The dataset used is the "Shop Customer Data" from Kaggle, containing 2,000 records with attributes such as age, annual income, spending score, profession, and more.

## Dataset Description
The dataset includes the following columns:
- **Customer ID**: Unique identifier for each customer.
- **Gender**: Customer's gender (Male/Female).
- **Age**: Customer's age.
- **Annual Income ($)**: Customer's yearly income.
- **Spending Score (1-100)**: Score assigned based on shopping behavior.
- **Profession**: Customer's profession.
- **Work Experience**: Years of work experience.
- **Family Size**: Number of family members.

## Project Steps
1. **Exploratory Data Analysis (EDA)**
   - Examined the dataset structure, missing values, and duplicates.
   - Visualized distributions of categorical and numerical features.
   - Conducted statistical analysis to understand data trends.

2. **Data Preprocessing**
   - Handled missing values by dropping null rows.
   - Encoded categorical variables (Gender, Profession) using label encoding.
   - Detected and managed outliers in numerical features.

3. **Clustering with K-Means**
   - Applied the Elbow Method and Silhouette Score to determine the optimal number of clusters (k=2).
   - Visualized clusters for features like Annual Income vs. Spending Score.
   - Experimented with different values of k (2, 3, 6) to compare results.

4. **Results Visualization**
   - Used Principal Component Analysis (PCA) to reduce dimensionality for plotting.
   - Created scatter plots to display customer clusters.

5. **Exporting New Dataset For Classification**
   
## Key Findings
- The optimal number of clusters was determined to be 2, with a Silhouette Score of 0.62.
- Clusters were visualized to highlight distinct customer segments based on income and spending behavior.
- Further analysis with k=3 and k=6 provided additional insights into customer groupings.



# Customer Classification Notebook

## Overview
This project focuses on classifying customers into predefined clusters using machine learning models. The goal is to evaluate different classification algorithms to predict customer segments based on demographic and behavioral features. The dataset used is derived from clustered customer data, which includes attributes such as age, annual income, spending score, and more.

## Dataset Description
The dataset contains the following columns:
- **Customer ID**: Unique identifier for each customer.
- **Gender**: Encoded customer's gender (0: Female, 1: Male).
- **Age**: Customer's age.
- **Annual Income ($)**: Customer's yearly income.
- **Spending Score (1-100)**: Score assigned based on shopping behavior.
- **Profession**: Encoded customer's profession.
- **Work Experience**: Years of work experience.
- **Family Size**: Number of family members.
- **Cluster**: Predefined customer segment (target variable).

## Project Steps
1. **Data Preparation**
   - Loaded the clustered customer dataset.
   - Split the data into training and testing sets (70:30 ratio).

2. **Model Training**
   - Trained four classification models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - K-Nearest Neighbors (K-NN)

3. **Model Evaluation**
   - Calculated evaluation metrics: Accuracy, F1-Score, Precision, and Recall.
   - Generated confusion matrices for each model to visualize performance.

4. **Results Analysis**
   - Compared the performance of all models.
   - Identified the best-performing classifiers.

## Key Findings
- **Logistic Regression**: Achieved an accuracy of 0.90, with balanced precision and recall.
- **Decision Tree, Random Forest, and K-NN**: All three models achieved perfect accuracy (1.00), indicating flawless classification on the test set.
- **Confusion Matrices**: Visualized the classification results, confirming the high performance of the models.


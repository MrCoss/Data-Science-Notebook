# Data Science Challenge Project

This repository documents an end-to-end data science project developed for the **Coursera "Data Science Challenge"** course. It demonstrates a complete workflow, including data cleaning, exploratory data analysis (EDA), predictive modeling, and insight generation, reflecting best practices in applied data science.

-----

## Table of Contents

  - [1. Project Context & Objectives](https://www.google.com/search?q=%231-project-context--objectives)
  - [2. The Data Science Methodology](https://www.google.com/search?q=%232-the-data-science-methodology)
  - [3. Key Findings & Recommendations](https://www.google.com/search?q=%233-key-findings--recommendations)
  - [4. Technical Stack](https://www.google.com/search?q=%234-technical-stack)
  - [5. Project Structure](https://www.google.com/search?q=%235-project-structure)
  - [6. How to Replicate](https://www.google.com/search?q=%236-how-to-replicate)
  - [7. Author](https://www.google.com/search?q=%237-author)

-----

## 1\. Project Context & Objectives

The goal of this project is to simulate a real-world data science task by taking a raw dataset and transforming it into actionable insights. This involves not only building a predictive model but also demonstrating the critical thinking and structured approach required to solve business problems with data.

### Core Objectives:

  - **Data Wrangling:** To process and clean a structured dataset, handling common issues like missing values, outliers, and skewed distributions.
  - **Exploratory Analysis:** To uncover hidden patterns, trends, and correlations within the data using statistical and visualization techniques.
  - **Predictive Modeling:** To build, train, and evaluate machine learning models to predict a target outcome.
  - **Insight Communication:** To effectively communicate findings and provide data-driven recommendations.

-----

## 2\. The Data Science Methodology

The project followed a structured, multi-stage approach to ensure robust and reliable results.

### Step 1: Data Cleaning & Preprocessing

  - **Handling Missing Values:** Missing data points were imputed using statistical measures (mean for numerical features, mode for categorical features) to preserve dataset integrity.
  - **Outlier Detection:** Identified and handled outliers to prevent them from skewing model training.
  - **Feature Scaling:** Applied **normalization** (e.g., `StandardScaler`) to continuous variables. This step is crucial for algorithms sensitive to feature scales and was found to significantly improve model performance.

### Step 2: Exploratory Data Analysis (EDA)

  - A thorough EDA was conducted to build intuition about the dataset.
  - **Visualizations** like correlation heatmaps, boxplots, and distribution plots were used to:
      - Identify relationships between variables.
      - Understand the distribution of each feature.
      - Visualize the relationships between features and the target variable.

### Step 3: Predictive Modeling

  - **Model Selection:** Two classic classification algorithms were implemented:
    1.  **Logistic Regression:** Chosen as a strong, interpretable baseline model.
    2.  **Decision Tree Classifier:** Selected for its ability to capture non-linear relationships and provide insight into feature importance.
  - **Hyperparameter Tuning:** Used **`GridSearchCV`** to systematically test different combinations of model parameters, ensuring the final models were optimized for the best possible performance.

### Step 4: Model Evaluation & Interpretation

  - **Performance Metrics:** Models were evaluated using **accuracy** for an overall performance snapshot and a **confusion matrix** to understand the types of errors (false positives vs. false negatives).
  - **Feature Importance:** The Decision Tree model was used to extract **feature importances**, identifying which variables were the most influential in predicting the outcome. This is a key step for translating model results into business insights.

-----

## 3\. Key Findings & Recommendations

  - **Impact of Preprocessing:** The analysis confirmed that data quality is paramount. Normalizing skewed continuous variables was the most impactful step, **improving model accuracy by approximately 20%**.
  - **Key Predictive Drivers:** Feature importance analysis revealed that a few key variables were disproportionately influential in the model's predictions, providing a clear focus for business strategy.
  - **Model Performance:** While both models performed well, the tuned Decision Tree slightly outperformed Logistic Regression, suggesting the presence of non-linear patterns in the data.
  - **Recommendations for Future Work:** For even better performance, further iterations should explore more complex models (e.g., Random Forest, Gradient Boosting) and experiment with more advanced feature engineering techniques.

-----

## 4\. Technical Stack

  - **Core Language:** Python 3.x
  - **Data Manipulation:** Pandas
  - **Data Visualization:** Matplotlib & Seaborn
  - **Machine Learning:** Scikit-learn
  - **Development Environment:** Jupyter Notebook

-----

## 5\. Project Structure

The project is contained within a single, well-documented Jupyter Notebook for ease of review and execution.

```
DataScienceChallenge/
├── DataScienceChallenge.ipynb      # The main notebook with all code, visualizations, and analysis.
└── README.md                     # This detailed documentation file.
```

-----

## 6\. How to Replicate

To view or run this project locally, please follow these steps.

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/MrCoss/Data-Science-Notebook.git
    cd Data-Science-Notebook
    ```
2.  **Set Up a Virtual Environment** (Recommended):
    ```bash
    # Create the environment
    python -m venv venv
    # Activate it
    # On Windows: .\venv\Scripts\activate
    # On macOS/Linux: source venv/bin/activate
    ```
3.  **Install Dependencies:**
    You will need `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, and `notebook`.
    ```bash
    pip install pandas matplotlib seaborn scikit-learn notebook
    ```
4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Navigate to `DataScienceChallenge.ipynb` in the Jupyter interface to open the notebook.

Alternatively, you can view the static notebook directly on GitHub:
**[View Notebook](https://github.com/MrCoss/Data-Science-Notebook/blob/main/DataScienceChallenge.ipynb)**

-----

## 7\. Author

  - **Pinto Costas Antony**
  - **GitHub Profile:** [MrCoss](https://github.com/MrCoss)

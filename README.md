# 📊 Amazon Product Price Prediction with Machine Learning

Welcome to the Amazon Product Price Prediction project! This repository contains an end-to-end machine learning project that analyzes Amazon product data and predicts prices based on features like ratings, reviews, and product categories. By implementing and comparing two powerful models, Random Forest and Linear Regression, this project aims to uncover insights into pricing strategies that can support e-commerce decision-making.

## 📂 Project Structure
```
├── data/                    # Folder for dataset
├── notebooks/               # Jupyter notebooks for analysis and model building
├── models/                  # Saved models for reuse
├── scripts/                 # R scripts for data processing, modeling, and evaluation
└── README.md                # Project overview and instructions
```

## 🌟 Key Features
- **Data Preprocessing**: Clean and prepare Amazon product data, removing unnecessary symbols and handling missing values.
- **Exploratory Data Analysis (EDA)**: Visualize data distributions, correlations, and price relationships.
- **Feature Engineering**: Enhance data with features like discount rate, price ratio, and review sentiment scores.
- **Model Training & Evaluation**: Build and evaluate Random Forest and Linear Regression models with metrics like RMSE and R².
- **Error Analysis**: Compare model performance with detailed error analysis, using visualization to assess accuracy.
  
## 📊 Dataset
This project uses an Amazon product dataset, which can be downloaded from [Kaggle](https://www.kaggle.com/code/mehakiftikhar/amazon-sales-dataset-eda/input).

### Columns in the Dataset
1. **product_id**: Unique identifier for each product
2. **product_name**: Descriptive product title
3. **category**: Product category hierarchy
4. **discounted_price**: Current selling price
5. **actual_price**: Original price before discounts
6. **discount_percentage**: Percentage of discount
7. **rating**: Customer rating (1 to 5 scale)
8. **rating_count**: Number of customer ratings
9. **about_product**: Product description
10. **review_content**: Content of customer reviews

📑 Dataset Column Descriptions
1.  **product_id**: Unique identifier for each product, enabling tracking and referencing of specific items.
2.  **product_name**: Name or title of the product, often including brand, type, and key features.
3.  **category**: Product category hierarchy, showing primary and sub-categories, separated by |.
4.  **discounted_price**: Selling price after discounts, originally formatted as a string with currency symbols.
5.  **actual_price**: Original price before any discounts, also formatted as a string with currency symbols.
6.  **discount_percentage**: Calculated percentage discount, based on the actual and discounted prices.
7.  **rating**: Average customer rating on a 1-5 scale, typically calculated from multiple reviews.
8.  **rating_count**: Total number of customer ratings, formatted as a string that may include commas.
9.  **about_product**: Detailed product description, often highlighting key features and benefits.
10. **user_id**: Unique identifiers of users who reviewed or rated the product, comma-separated for multiple users.
11. **user_name**: Names of users who reviewed or rated the product, listed as comma-separated values.
12. **review_id**: Unique identifiers for each review, provided as a comma-separated list.
13. **review_title**: Brief summary or title of each review, giving an impression of the review content.
14. **review_content**: Full content of each review, containing detailed opinions and feedback from users.
15. **img_link**: URL link to the product’s image, hosted on Amazon’s servers.
16. **product_link**: Direct URL link to the product’s listing on Amazon, allowing easy access for further details or purchasing.

## 🚀 Getting Started

### Prerequisites
To run this project, you’ll need:
- **R** with packages: `dplyr`, `ggplot2`, `caret`, `randomForest`, `Metrics`, `reshape2`
- **RStudio** (optional, for interactive analysis)

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/username/repo-name.git
   ```
2. Install the required R packages:
   ```R
   install.packages(c("dplyr", "ggplot2", "caret", "randomForest", "Metrics", "reshape2"))
   ```

3. Download the dataset and place it in the `data/` folder.

## 📝 Project Workflow

1. **Data Cleaning & Preprocessing**: Clean the data and transform variables for analysis.
2. **Exploratory Data Analysis**: Generate visualizations to understand data patterns.
3. **Feature Engineering**: Create new features to enhance model performance.
4. **Model Training**:
   - **Random Forest**: Trained using cross-validation to capture non-linear relationships.
   - **Linear Regression**: Provides interpretable results with confidence intervals.
5. **Model Evaluation**: Assess accuracy using RMSE, R², and error distributions.
6. **Error Analysis**: Visualize model errors to identify improvement areas.

## 📈 Results
The Random Forest model outperformed Linear Regression, showing lower RMSE and higher R² scores, indicating better handling of non-linear relationships in product pricing. Feature importance analysis revealed that actual price, rating, and category have a strong impact on predicted prices.

## 🔍 Insights & Future Work
- **Insights**: Products with higher actual prices and ratings tend to have higher discounted prices, suggesting that pricing is closely related to perceived quality.
- **Future Work**: Explore additional models like XGBoost, incorporate more text analysis on reviews, and create an interactive dashboard for user engagement.

## 📬 Contact
For questions or feedback, please reach out at **your.email@example.com**.

---

**Thank you for exploring the Amazon Product Price Prediction project!** 👋

---

This README file offers a structured overview of your project, making it easy to understand the purpose, setup, and workflow.

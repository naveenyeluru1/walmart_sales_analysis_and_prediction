# Walmart Store Sales Forecasting

## Project Overview

This project aims to analyze and predict weekly sales for Walmart stores based on various features such as store type, department, geographical data, economic factors, and holiday information. The dataset used in this project consists of historical sales data, store information, and additional features related to economic conditions and holidays.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)

## Data Description

- `stores.csv`: Contains information about the stores, including store type and size.
- `train.csv.zip`: Contains historical sales data, including store, department, date, weekly sales, and holiday information.
- `test.csv.zip`: Contains test data for making predictions.
- `features.csv.zip`: Contains additional features such as temperature, fuel price, and economic indicators.

## Data Preprocessing

Data preprocessing includes:
- Reading the CSV files into DataFrames.
- Merging datasets to create a comprehensive dataset for analysis.
- Dropping unnecessary columns and handling missing values.
- Removing outliers and ensuring data consistency.

## Exploratory Data Analysis

- Analyzing the distribution of store types and their sales contributions.
- Investigating the impact of holidays on sales.
- Examining trends and patterns in sales data over time.
- Generating correlation heatmaps to understand relationships between variables.

## Feature Engineering

- Extracting year and month from the date for temporal analysis.
- Label encoding categorical variables such as `IsHoliday` and `Type`.
- Creating additional features like `month` for seasonal analysis.

## Model Training and Evaluation

- Splitting the data into training and testing sets.
- Training various models including DecisionTreeRegressor, RandomForestRegressor, and XGBRegressor.
- Evaluating models using metrics such as R2 score, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
- Hyperparameter tuning and model selection based on evaluation metrics.

## Results

- **Best Model**: XGBRegressor achieved the highest R2 score and lowest RMSE.
- **Evaluation Metrics**:
  - R2 score: 0.926
  - MSE: 38,406,152
  - RMSE: 6,197.27

## Visualization

- Bar plots to visualize the distribution of store types and their sales.
- Line plots for temporal analysis of sales data.
- Correlation heatmaps to understand relationships between features.
- Feature importance plots to identify key predictors of sales.

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This README provides a comprehensive overview of the project, from data preprocessing and exploratory data analysis to model training and evaluation. It ensures that anyone interested in the project can easily understand and replicate the process.

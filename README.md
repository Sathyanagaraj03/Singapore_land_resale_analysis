# Singapore Land Resale Price Prediction using Machine Learning

![Model Evaluation](https://singaporenewproperty.net/wp-content/uploads/2023/07/Property-News-800x445.jpg)

This project aims to predict the resale prices of land in Singapore using machine learning models. By analyzing historical data on land resale transactions, we will build predictive models to help forecast future land prices. The analysis includes data preprocessing, model training, evaluation, and prediction.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Methodology](#methodology)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Results](#results)
8. [Future Work](#future-work)
9. [Contributing](#contributing)
10. [License](#license)

---

## Project Overview

Real estate prices in Singapore are highly influenced by factors such as location, property size, and economic trends. This project leverages machine learning to predict the resale prices of land in Singapore based on historical resale data and various features such as property type, area, age, and proximity to amenities.

---

## Dataset

The dataset used for this project includes historical resale transaction data from sources such as:

Key features include:
- **Location** (district, postal code, proximity to MRT)
- **Land Size** (square meters)
- **Property Type** (HDB, condo, landed)
- **Age of Property**
- **Resale Price**
- **Year of Transaction**

---

## Installation

### Requirements

To run the project, you need the following installed:

- Python 3.8+
- Jupyter Notebook (optional)
- Libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`


### Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/sathyanagaraj03/singapore-land-resale-prediction.git
    cd singapore-land-resale-prediction
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

---

## Methodology

1. **Data Collection**: We aggregate data from multiple sources on resale prices, land details, and amenities.
2. **Data Preprocessing**:
   - Handle missing values
   - Normalize and scale numeric data
   - Convert categorical features to numerical values using one-hot encoding
3. **Feature Engineering**: Create new features such as proximity to MRT stations, number of schools within a 1km radius, and more.
4. **Model Training**: We split the data into training and test sets, applying various machine learning models.
5. **Evaluation**: Use RMSE, MAE, and R² scores to evaluate model performance.

## Modeling

We experiment with several machine learning models, including:

1. **Linear Regression**
2. **Decision Tree Regression**
3. **Random Forest**

## Evaluation

Model performance is evaluated using:

- **Mean Absolute Error (MAE)**
- **Root Mean Square Error (RMSE)**
- **R² Score**

The best-performing model is selected based on its ability to generalize well on unseen test data.

---

## Results

- **Best Model**: Random Forest with RMSE of 120,000 SGD and R² score of 0.85 on the test set.
- **Feature Importance**: The most significant features for predicting resale price include:
  - Location (district)
  - Property Type (HDB, landed, condo)
  - Land size
  - Age of property

---

## Future Work

Potential improvements and future work for the project include:
- Incorporating more granular location data (e.g., specific amenities).
- Using more advanced models like Gradient Boosting or deep learning models.
- Enhancing feature engineering, especially for geographic-based variables.
- Adding time series analysis to capture market trends.

---

## Contributing

We welcome contributions to this project. If you'd like to contribute, please:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a Pull Request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.



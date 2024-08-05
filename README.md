# Insurance Premium Prediction

## Overview

This project aims to estimate individual healthcare costs to help customers focus on the health benefits of insurance plans. The project involves developing APIs using Flask, optimizing model performance with GridSearchCV and Cross-Validation, and implementing data preprocessing, feature engineering, and visualization to enhance accuracy and provide actionable insights. It is deployed on AWS Elastic Beanstalk and CodePipeline for end-to-end machine learning deployment.

## Problem Statement

The goal of this project is to provide individuals with an estimate of their healthcare costs based on their unique health situations. This estimate can assist customers in focusing on the health benefits of various insurance plans rather than the cost aspect. By understanding their potential expenses, customers can make more informed decisions when selecting an insurance policy.

## Dataset

The dataset used in this project is sourced from Kaggle. It contains information on insurance premiums and the factors affecting them. You can download it from [here](https://www.kaggle.com/noordeen/insurance-premium-prediction).

## Approach

### 1. Data Exploration
- **Tools:** Pandas, NumPy, Matplotlib, Plotly, Seaborn
- **Description:** Exploring the dataset to understand its structure and characteristics. This step involves loading the dataset and performing initial inspections, such as checking for missing values, data types, and basic statistics.

### 2. Exploratory Data Analysis (EDA)
- **Tools:** Matplotlib, Seaborn, Plotly
- **Description:** Plotting various graphs to gain insights into dependent and independent variables/features. This includes visualizing distributions, relationships, and correlations between variables to identify patterns and potential outliers.

### 3. Feature Engineering
- **Techniques:** Scaling numerical features, encoding categorical features
- **Description:** Preparing the dataset for modeling by transforming features. This step involves handling missing values, creating new features, transforming existing ones, and encoding categorical variables using techniques such as one-hot encoding.

### 4. Model Building
- **Techniques:** Dataset splitting, training on multiple algorithms
- **Description:** Splitting the dataset into training and testing sets, and training the model on various algorithms. The models used include:
  1. **Linear Regression:** A simple and interpretable model.
  2. **Decision Tree Regressor:** A tree-based model that splits the data into regions.
  3. **Random Forest Regressor:** An ensemble model that builds multiple decision trees.
  4. **Gradient Boosting Regressor:** An ensemble model that builds trees sequentially to minimize errors.
  5. **XGBoost Regressor:** An optimized version of gradient boosting.

### 5. Model Selection
- **Metrics:** RMSE, R-squared
- **Description:** Evaluating models based on performance metrics such as Root Mean Squared Error (RMSE) and R-squared. The model with the best performance is selected for deployment.

### 6. Pickle File
- **Description:** Creating a pickle file of the selected model for later use. This allows the model to be loaded and used without retraining.

### 7. Webpage & Deployment
- **Tools:** Flask, HTML, CSS
- **Description:** Developing a web application that takes user inputs and displays predicted insurance premiums. The application is deployed on AWS Elastic Beanstalk for scalable and reliable hosting.

## Deployment Link

[Insurance Premium Prediction Web Application](http://insurance-premium-prediction-env.eba-cnranump.eu-north-1.elasticbeanstalk.com/)

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-Learn
- Flask
- HTML
- CSS

## Technical Aspects

- **Programming Language:** Python
- **Front-end:** HTML, CSS
- **Back-end:** Flask
- **Deployment:** AWS Elastic Beanstalk and CodePipeline

## Repository Structure

```plaintext
.
├── .ebextensions         # Deployment configurations
├── artifacts             # Artifacts and requirements
├── documents1            # Project documents
├── notebooks             # Jupyter notebooks for EDA and model building
├── src                   # Source code for the application
├── templates             # HTML templates for the Flask application
├── .gitignore            # Git ignore rules
├── README.md             # Project documentation
├── application.py        # Flask application file
├── requirements.txt      # Project dependencies
├── setup.py              # Setup script for the project
```

## Getting Started

### Prerequisites

- Python 3.8 or higher
- AWS account for deployment

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/GourangPatidar/Insurance-Premium-Prediction.git
   cd Insurance-Premium-Prediction
   ```

2. **Install the dependencies**
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

Run the application using the following command:
```bash
python application.py
```

## Contributing

We welcome contributions to improve and expand this project. Please follow the steps below to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Create a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Kaggle for providing the dataset.
- The open-source community for their invaluable contributions.

---



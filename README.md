# Forest Fire Prediction Model

This project aims to predict forest fire occurrences using various regression techniques. The dataset used contains data related to forest fires, and the project explores the data, applies feature engineering, and uses different machine learning models to predict the likelihood of forest fires. The model that achieved the highest accuracy is Ridge Regression with 98%.

## Project Structure

- **notebooks/**  
  Contains Jupyter Notebooks used for data exploration and model training.
  - **ForestFireModel.ipynb**: Data cleaning, feature engineering, and exploratory data analysis (EDA) are performed here.
  - **Model_Training.ipynb**: Model training and comparison of regression techniques. It focuses on correlation analysis to select the best features for prediction.

- **templates/**  
  Contains HTML files for the web interface.
  - **home.html**: The main user interface where users can input data and predict the likelihood of a forest fire.

- **app.py**: The Flask application that connects the trained model to the web interface.

## Installation and Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/PremKr1122/forestfires
    cd forest-fire-prediction
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Flask application:
    ```bash
    python app.py
    ```

5. Access the user interface by opening your browser and navigating to `http://localhost:5000`.

## Data Exploration and Feature Engineering

The **ForestFireModel.ipynb** notebook performs:

- **Data Cleaning**: Handle missing values and preprocess the dataset.
- **Exploratory Data Analysis (EDA)**: Visualizes the data to understand relationships between features and the target variable.
- **Feature Engineering**: Creates new features that could improve model predictions.

## Model Training and Evaluation

In the **Model_Training.ipynb** notebook, the following steps are performed:

- **Correlation Analysis**: Identifies the most important features for predicting forest fires.
- **Model Comparison**: Compares the performance of multiple regression models, including Linear Regression, Ridge Regression, and others.
- **Ridge Regression**: Achieved an accuracy of 98%, making it the most accurate model in this project.

## Flask Web Interface

- **home.html**: The user interface allows users to input features such as temperature, humidity, wind speed, etc., and predicts the likelihood of a forest fire.
- **app.py**: The Flask backend that serves the model and interfaces with the frontend.

## Conclusion

This project demonstrates how to predict forest fires using machine learning models, with Ridge Regression achieving the highest accuracy. The Flask web interface makes the model easily accessible for users to input data and get predictions.

![Interfcace of the Model](https://github.com/PremKr1122/forestfires/blob/main/FFP_Output.png?raw=true)


# Medical Insurance Price Prediction with Machine Learning

[](https://opensource.org/licenses/MIT)
[](https://www.python.org/downloads/)
[](https://scikit-learn.org/)

A machine learning project to predict individual medical insurance premium costs based on their demographic and health attributes.

-----

## 📝 Description

This project aims to build a machine learning model that can predict the annual health insurance premium costs billed to an individual. By using data such as age, gender, body mass index (BMI), number of children, smoking status, and region of residence, this model provides a cost estimate that can assist insurance companies in pricing and potential customers in forecasting their expenses.

## 🎯 Problem Background

Determining insurance premium prices is a complex process that depends on many risk factors. For insurance companies, accurate estimation is crucial for maintaining profitability and competitiveness. On the other hand, for potential customers, understanding which factors most influence premium costs can help them make better decisions regarding their lifestyle and policy choices. This project attempts to bridge that gap by creating a transparent and reliable prediction model.

## ✨ Key Features

  - **Exploratory Data Analysis (EDA)**: A Jupyter Notebook containing in-depth analysis and data visualization to understand the relationships between variables.
  - **Data Preprocessing**: Implementation of techniques like One-Hot Encoding to handle categorical features.
  - **Model Training**: Utilizes several regression models to find the most accurate one, with a focus on Gradient Boosting.
  - **Performance Evaluation**: Measures model accuracy using standard regression metrics like MAE, MSE, and R-squared ($R^2$).

## 📊 Dataset

The model is trained using the popular "Medical Cost Personal Datasets" available on Kaggle. You can download it from [here](https://www.kaggle.com/datasets/mirichoi0218/insurance).

This dataset has 7 feature columns:

  - `age`: Age of the primary beneficiary.
  - `sex`: Gender of the insurance contractor (female, male).
  - `bmi`: Body Mass Index.
  - `children`: Number of children covered by health insurance / Number of dependents.
  - `smoker`: Smoking status (yes, no).
  - `region`: The beneficiary's residential area in the US (northeast, southeast, southwest, northwest).
  - `charges`: **(Target)** Individual medical costs billed by health insurance.

## 🛠️ Tech Stack

  - **Programming Language**: Python 3.8+
  - **Analysis & Computation Libraries**: Pandas, NumPy
  - **Visualization Libraries**: Matplotlib, Seaborn
  - **Machine Learning Libraries**: Scikit-learn (for preprocessing and models), XGBoost
  - **Environment**: Jupyter Notebook


## 🤖 Model and Evaluation

Various regression models were explored, including Linear Regression, Random Forest, and Gradient Boosting. The **Gradient Boosting Regressor** model provided the best results due to its ability to handle complex interactions between features.

Before training, categorical data (`sex`, `smoker`, `region`) were transformed using One-Hot Encoding.

The model's performance was evaluated on the test data using the following metrics:

  - **Mean Absolute Error (MAE)**: The average of the absolute errors.
  - **Mean Squared Error (MSE)**: The average of the squared errors.
  - **R-squared ($R^2$)**: The coefficient of determination.

The final model achieved an **$R^2$ score of approximately 0.85**, indicating that the model can explain about 85% of the variability in the insurance cost data.

## 🤝 Contributing

Contributions are very welcome\! If you'd like to contribute to this project, please follow these steps:

1.  **Fork** this repository.
2.  Create a new **Branch** for your feature (`git checkout -b feature/CoolFeature`).
3.  Make your changes and **Commit** them (`git commit -m 'Add some CoolFeature'`).
4.  **Push** to your Branch (`git push origin feature/CoolFeature`).
5.  Create a new **Pull Request** and describe your changes.

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

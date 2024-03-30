# Employee Absenteeism Prediction Model

This project aims to build a machine learning model to predict employee absenteeism using various features such as transportation expense, age, body mass index, education level, and reasons for absence. The model can help organizations understand the factors contributing to employee absenteeism and take appropriate measures to address it.

## Project Overview

The project consists of the following main components:

1. **Data Preprocessing**: The raw data is cleaned, transformed, and feature engineered to prepare it for model training.
2. **Model Training**: A logistic regression model is trained on the preprocessed data to predict employee absenteeism.
3. **Model Evaluation**: The trained model is evaluated on a test set to assess its performance.
4. **Model Deployment**: The trained model and the scaler used for data preprocessing are saved for future use in predicting absenteeism on new data.

## File Structure

- `Absenteeism_DA.ipynb`: Jupyter Notebook containing the data preprocessing steps.
- `Absenteeism_Logistic_Regression.ipynb`: Jupyter Notebook containing the logistic regression model training and evaluation.
- `absenteeism_module.py`: Python script containing the `absenteeism_model` class, which loads and preprocesses the data, trains the model, and provides methods for making predictions on new data.
- `model`: A serialized file containing the trained machine learning model.
- `scaler`: A serialized file containing the scaler used for data preprocessing.
- `README.md`: This file, providing an overview of the project.

## Usage

1. Clone the repository or download the project files.
2. Install the required Python libraries (NumPy, Pandas, Scikit-learn, Pickle).
3. Import the `absenteeism_model` class from `absenteeism_module.py`.
4. Create an instance of the `absenteeism_model` class, providing the paths to the `model` and `scaler` files.
5. Load and preprocess your new data using the `load_and_clean_data` method.
6. Use the `predicted_probability`, `predicted_output_category`, or `predicted_outputs` methods to obtain predictions on the new data.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

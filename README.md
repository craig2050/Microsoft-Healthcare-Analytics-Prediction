
# Hospital Stay Prediction Using Machine Learning

## Project Overview

Predicting the length of hospital stays is essential for effective resource management in healthcare. By forecasting patient stay durations, hospitals can allocate resources more efficiently, reduce patient wait times, and enhance care quality. This project demonstrates how machine learning models can be used to predict hospital stays using real-world healthcare data.

The project explores the entire data science pipeline, from data cleaning to model deployment, emphasizing the importance of accurate predictions in life-critical scenarios. The outcome of this project can help hospitals optimize their operations and patient management strategies.

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Data Cleaning](#data-cleaning)
- [Data Analytics](#data-analytics)
- [Model Building](#model-building)
- [Final Model](#final-model)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run this project, ensure you have the following libraries installed:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Data Cleaning

The dataset underwent thorough cleaning to ensure data quality:
- **Handling Missing Values**: Filled or removed missing data to ensure a complete dataset.
- **Data Integrity Checks**: Ensured that the data remained consistent and accurate throughout the process.

## Data Analytics

Several key analyses were performed:
- **Univariate Analytics**: Examined the distribution and behavior of individual variables.
- **Correlation and Associations**: Identified relationships between variables to uncover impactful patterns.
- **Feature Engineering**: Created new features to improve predictive accuracy.
- **Feature Importance with Random Forest**: Determined the most influential features for the model.

## Model Building

Two main iterations were conducted to refine the model:
1. **Iteration 1 - Initial Barebones Model**: A baseline model was built to establish a starting point.
2. **Iteration 2 - Grid Search and Hyperparameter Tuning**: 
   - Used Grid Search to identify the best parameters for the model.
   - Evaluated training vs. testing accuracy to avoid overfitting.

### Model Performance Evaluation:
- Train vs Test Accuracy plots were generated to monitor overfitting.
  
## Final Model

The final model was built using the best hyperparameters found through grid search. The model was saved as a pickle file for future use and can be loaded to make predictions on new data.

## Usage

To use the final model, load the pickle file and pass new data to generate predictions. Example:

```python
import pickle

# Load the model
with open('final_model.pkl', 'rb') as file:
    model = pickle.load(file)

# Predict new data
predictions = model.predict(new_data)
```

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you would like to improve this project.

## License

This project is licensed under the MIT License - see the [LICENSE](#https://microsoft.github.io/r-server-hospital-length-of-stay/index.html) file for details.

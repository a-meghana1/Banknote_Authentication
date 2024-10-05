# Banknote Authentication Project

This project aims to build a model that can classify banknotes as genuine or counterfeit using the Banknote Authentication Dataset from Kaggle.

## Data Exploration and Preprocessing

*   Loaded the dataset and inspected its structure and information.
*   Renamed columns for clarity.
*   Checked for missing values and ensured data integrity.
*   Performed Exploratory Data Analysis (EDA) using visualizations and descriptive statistics.
*   Investigated the relationship between features and the target variable (Class).
*   Used box plots and histograms to understand data distribution and identify potential outliers.

## Feature Selection and Engineering

*   Calculated the correlation between features and the target variable.
*   Identified important features (Variance, Skewness, Kurtosis) based on correlation and statistical significance.
*   Removed the "Entropy" feature due to its low significance.
*   Split the data into training and testing sets.
*   Applied StandardScaler to standardize the features.

## Model Selection, Training, and Evaluation

*   Chose Logistic Regression as the classification model.
*   Trained the model using the training data.
*   Evaluated the model's performance using metrics like accuracy, precision, recall, and F1-score on the testing data.
*   Generated a confusion matrix to visualize the model's predictions.
*   Explored adjusting the prediction threshold to optimize precision and recall trade-offs.

## Usage

To run the notebook:

1.  Upload the notebook to Google Colab.
2.  Install necessary libraries using `!pip install library_name`.
3.  Load the dataset by updating the file path in `pd.read_csv('/content/data_banknote_authentication.csv')`.
4.  Run the cells sequentially.

## Key Findings

*   Variance, Skewness, and Kurtosis were found to be significant features for classifying banknotes.
*   The model achieved high accuracy in classifying genuine and counterfeit banknotes.

## Future Improvements

*   Explore other classification models (e.g., Random Forest, SVM).
*   Fine-tune hyperparameters to improve model performance.
*   Implement cross-validation for robust evaluation.

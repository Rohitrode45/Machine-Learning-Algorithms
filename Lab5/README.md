# Decision Tree Classifier on Drug Dataset

This project demonstrates how to implement a Decision Tree Classifier to predict the type of drug recommended for a patient based on their medical information, such as age, sex, blood pressure, cholesterol level, and sodium-to-potassium ratio.

## Project Overview

The project is structured as a Jupyter Notebook and includes the following steps:

1. **Importing Libraries**: The necessary libraries for data manipulation, model training, and evaluation are imported.
2. **Loading the Dataset**: The dataset containing patient medical records is loaded from a CSV file and previewed.
3. **Data Preprocessing**: Categorical features like gender, blood pressure, and cholesterol levels are encoded into numerical format using Label Encoding.
4. **Splitting Data into Features and Target**: The data is split into features (Age, Sex, BP, Cholesterol, Na_to_K) and target (Drug). The dataset is then split into training and testing sets.
5. **Training the Model**: A Decision Tree Classifier is trained on the training data.
6. **Model Evaluation**: The model is evaluated using accuracy and a classification report, which provides precision, recall, and F1-score for each drug type.

## Dataset

The dataset used in this project contains the following columns:

- **Age**: Age of the patient
- **Sex**: Gender of the patient (M/F)
- **BP**: Blood pressure level (HIGH, LOW, NORMAL)
- **Cholesterol**: Cholesterol level (HIGH, NORMAL)
- **Na_to_K**: Ratio of sodium to potassium in the blood
- **Drug**: The type of drug recommended (drugY, drugC, drugA, etc.)

### Example Rows:

| Age | Sex | BP      | Cholesterol | Na_to_K | Drug |
|-----|-----|---------|-------------|---------|------|
| 23  | F   | HIGH    | HIGH        | 25.355  | drugY|
| 47  | M   | LOW     | HIGH        | 13.093  | drugC|
| 28  | F   | NORMAL  | HIGH        | 7.798   | drugX|

## Getting Started

### Requirements

- Python 3.x
- Jupyter Notebook or Google Colab
- Required Libraries:
  - pandas
  - scikit-learn

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/decision-tree-drug-classifier.git

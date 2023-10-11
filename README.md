# Spam-Detector

## Description

This repository contains a Python script for a spam message classifier. The script reads a dataset of text messages labeled as either "spam" or "ham" (non-spam), processes the text data, trains a Naive Bayes classifier, and evaluates the model's performance.

![image](https://github.com/Aditya3012Purwar/Spam-Detector/assets/103439955/8ac491b2-5765-4e1a-82ad-7ffc053d4fde)


## Requirements

- Python
- NumPy
- pandas
- NLTK
- scikit-learn

## Dataset

The dataset is a CSV file (`spam.csv`) containing text messages and their corresponding labels ("spam" or "ham"). It has been pre-processed to remove duplicates and unnecessary columns, resulting in a clean dataset ready for model training.

## How the Script Works

1. **Import Required Libraries:**
   - The script starts by importing necessary libraries including NumPy, pandas, NLTK, and scikit-learn.

2. **Load the Dataset:**
   - Reads the `spam.csv` file into a pandas DataFrame, drops unnecessary columns, and renames the remaining columns for better readability.

3. **Text Pre-processing:**
   - The `process_text` function is defined to remove punctuation and stopwords from the text messages. The cleaned text is then tokenized.

4. **Vectorization:**
   - The cleaned text messages are converted into a matrix of token counts using `CountVectorizer`.

5. **Train-Test Split:**
   - The dataset is split into training and testing sets (80% training, 20% testing).

6. **Model Training:**
   - A Multinomial Naive Bayes classifier is trained on the training dataset.

7. **Model Evaluation:**
   - The model's performance is evaluated using the training set, and metrics like precision, recall, and accuracy are printed.
   - The model is then evaluated using the testing set, and similar metrics are printed to observe the model's performance.

## Results

The model achieved an accuracy of approximately 99.5% on the training dataset and 95.5% on the testing dataset, indicating a highly effective spam filter.

## Usage

Ensure you have all the required libraries installed. You can run the script using any Python IDE or command-line interface. Make sure the `spam.csv` dataset is in the correct path or update the path accordingly in the `pd.read_csv` function.

## Support

For any issues or improvements, feel free to contribute to the code or contact the repository owner.

--- 

# 🎬 Movie Genre Classification

## 📌 Project Overview
This project implements a machine learning model to predict the genre of a movie based on its plot summary. The solution tackles a multi-class text classification problem using Natural Language Processing (NLP) techniques.

## 📊 Dataset
**Source:** [IMDb Genre Classification Dataset (Kaggle)](https://www.kaggle.com/datasets/hijest/genre-classification-dataset-imdb)
* **train_data.txt:** Labeled movie plots for training.
* **test_data.txt:** Unlabeled plots for prediction.
* **test_data_solution.txt:** Ground truth for evaluation.

## 🛠 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Scikit-learn, NLTK
* **Model:** Multinomial Naive Bayes

## ⚙️ Methodology
1.  **Data Loading:** Parsed non-standard text files using custom separators (`::: `).
2.  **Preprocessing:**
    * Lowercasing and removing special characters.
    * Stopword removal and Stemming (LancasterStemmer).
3.  **Feature Engineering:** TF-IDF Vectorization (Top 5000 features).
4.  **Model Training:** Trained a Naive Bayes classifier on the processed text.
5.  **Evaluation:** Tested against the solution file to calculate accuracy.

## 📈 Results
* **Accuracy:** ~51-54% (Baseline for 27 distinct genres)
* **Best Performance:** Western, Documentary, and Sport genres.
* **Challenges:** High overlap between generic genres like Drama and Romance.

## 🚀 How to Run
1.  Install dependencies: `pip install -r requirements.txt`
2.  Download the dataset and place the `.txt` files in the project root.
3.  Run the notebook:
    ```bash
    jupyter notebook Movie_Genre_Classification.ipynb
    ```
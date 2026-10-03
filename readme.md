# 🎵 Music Mood Prediction

## 📌 Project Overview

This project uses Machine Learning to predict the mood of a song based on its audio features.

The project analyzes music characteristics such as **tempo, energy, danceability, valence, and acousticness** and uses them to classify songs into different mood categories.

The Machine Learning models used in this project are:

* Logistic Regression
* Decision Tree
* Random Forest

## 🎯 Objective

The main objective of this project is to build a Machine Learning model that can predict the mood of a song from its audio features.

The project also compares the performance of different classification algorithms using:

* Accuracy
* Precision
* Recall
* Confusion Matrix
* Classification Report

## 📊 Dataset

The dataset contains **500 songs** with the following columns:

| Feature        | Description                 |
| -------------- | --------------------------- |
| `song`         | Name/identifier of the song |
| `tempo`        | Tempo of the song           |
| `energy`       | Energy level                |
| `danceability` | Danceability value          |
| `valence`      | Musical positivity/valence  |
| `acousticness` | Acousticness value          |
| `mood`         | Target mood category        |

The mood categories in the dataset are:

* Angry
* Sad
* Energetic
* Calm
* Happy
* Relaxed

The dataset contains 500 rows and 7 columns.

## 🛠️ Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* Jupyter Notebook

## 🔄 Project Workflow

1. Upload the CSV dataset.
2. Load the dataset using Pandas.
3. Clean the column names.
4. Identify the target mood column.
5. Check the dataset and its dimensions.
6. Check for missing values and duplicate rows.
7. Select the required audio features.
8. Split the data into training and testing sets.
9. Train multiple Machine Learning models.
10. Evaluate the models using accuracy, precision, and recall.
11. Visualize model performance.
12. Generate a confusion matrix and classification report.
13. Predict the mood of a new song.

The dataset is split into **80% training data and 20% testing data**.

## 🤖 Machine Learning Models

### 1. Logistic Regression

Logistic Regression is used as one of the classification models. A `StandardScaler` is included in a Pipeline before the Logistic Regression model.

### 2. Decision Tree

A Decision Tree classifier is trained to predict the mood category of a song.

### 3. Random Forest

A Random Forest classifier with 100 estimators is also trained for mood prediction.

## 📈 Model Results

The models produced the following results on the test data:

| Model               | Accuracy | Precision | Recall |
| ------------------- | -------: | --------: | -----: |
| Logistic Regression |   85.00% |    85.39% | 85.00% |
| Decision Tree       |   78.00% |    78.11% | 78.00% |
| Random Forest       |   85.00% |    85.66% | 85.00% |

These results are from the 100-record test set used in the notebook.

## 📉 Visualizations

The project generates visualizations for:

* Model Accuracy
* Model Precision
* Model Recall
* Random Forest Confusion Matrix

The confusion matrix is used to compare the actual and predicted mood classes.

## 🎵 New Song Prediction

The project also demonstrates how to predict the mood of a new song using five input features:

```text
Tempo
Energy
Danceability
Valence
Acousticness
```

The trained Random Forest model is used for the example prediction.

## 🚀 How to Run

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Run the notebook cells from top to bottom.
3. When prompted, upload the CSV dataset.
4. The notebook will preprocess the data, train the models, evaluate their performance, and generate predictions.

### Option 2: Local Python Environment

Install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

Then open and run the Jupyter Notebook:

```bash
jupyter notebook
```

## 📁 Project Structure

```text
music-mood-prediction/
│
├── music_mood_prediction.ipynb
├── song_ml_dataset_500.csv
├── README.md
└── requirements.txt
```

## 📌 Conclusion

This project demonstrates how Machine Learning can be applied to music audio features to classify songs into different mood categories.

Three classification algorithms were tested, and their performance was evaluated using accuracy, precision, and recall. The project also includes visualizations, a confusion matrix, a classification report, and an example of predicting the mood of a new song.

## 👤 Author
kavya vyas

---

⭐ If you found this project useful, consider giving the repository a star!

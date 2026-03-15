# Project Structure

This project is organized into several notebooks, each responsible for a specific stage of the machine learning pipeline. The workflow follows a typical natural language processing process: **exploration → preprocessing → training → evaluation**.

## 1. EDA Notebook (`EDA.ipynb`)

The **EDA (Exploratory Data Analysis)** notebook contains the initial exploration of the dataset.  
In this stage, the structure and characteristics of the tweets are analyzed to better understand the data.

The analysis includes:

- Distribution of tweet lengths
- Token length distribution
- Hashtag, mention, and URL analysis
- Stopword and content-word comparison
- Punctuation and capitalization patterns
- Language detection
- Non-ASCII character inspection
- Geographic information analysis
- Class distribution and imbalance inspection

These analyses help identify potential issues in the dataset and guide the design of the preprocessing and modeling steps.

---

## 2. Cleaning Notebook (`Cleaning.ipynb`)

The **Cleaning notebook** is responsible for preparing the dataset before training the models.

The preprocessing pipeline includes:

- Removing duplicate tweets
- Removing emojis and non-standard characters
- Removing URLs, mentions, and special symbols
- Converting text to lowercase
- Removing punctuation and unnecessary characters
- Removing stopwords
- Performing lemmatization to reduce words to their base form

After the preprocessing steps are applied, a **clean version of the dataset** is generated and saved for use in the training phase.

---

## 3. Training Notebook (`Training.ipynb`)

The **Training notebook** loads the cleaned dataset and trains the machine learning models.

The workflow in this notebook includes:

- Loading the cleaned dataset
- Splitting the dataset into **training, validation, and testing sets**
- Tokenizing the text and converting tweets into numerical sequences
- Applying padding to ensure uniform sequence length
- Training different model configurations, including neural network architectures

The models are trained using standard optimization techniques and evaluated using classification metrics.

---

## 4. Results Notebook (`Results.ipynb`)

The **Results notebook** compares the performance of the different models trained in the previous stage.

The evaluation includes:

- Accuracy
- Precision
- Recall
- F1-score
- AUC (Area Under the Curve)

Additionally, visualizations such as **confusion matrices and metric comparison plots** are generated to analyze the strengths and weaknesses of each configuration.

This notebook provides the final comparison and interpretation of the models’ performance.



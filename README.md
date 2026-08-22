# 🎬 Task 4: Movie Rating Prediction using Machine Learning

## 📌 Executive Summary
Movie rating prediction is a classic Supervised Machine Learning problem that helps film studios, streaming platforms, and investors estimate how well a movie will perform based on historical data. 

This project aims to build a **Regression Model** that predicts a movie's **IMDb Rating** using structural parameters such as genre, director, runtime, voting volume, and box-office revenue.

---

## 🗂️ Dataset Details
* **Dataset Name:** IMDb Movie Data
* **Data Source:** IMDb / Kaggle
* **Target Variable:** `Rating` (Continuous numerical score from 1.0 to 10.0)
* **Key Features:**
  * `Genre`: Category/style of the movie (e.g., Action, Drama, Comedy)
  * `Director`: Director of the film
  * `Runtime (Minutes)`: Total duration of the movie
  * `Votes`: Total number of user votes received on IMDb
  * `Revenue (Millions)`: Gross box-office collection in millions

---

## ⚙️ Technical Workflow & Methodology

### 1. Data Loading & Preprocessing
* Loaded dataset into a `pandas` DataFrame.
* Handled missing values (`NaN`) across features.
* Encoded categorical features (`Genre`, `Director`) into numerical values using `LabelEncoder`.

### 2. Feature Selection & Splitting
* Defined independent variables ($X$) and target variable ($y = \text{Rating}$).
* Split data into **80% Training Set** and **20% Testing Set** using `train_test_split`.

### 3. Model Implementation
* Implemented the **Random Forest Regressor** algorithm, an ensemble model using multiple decision trees to reduce overfitting and improve prediction accuracy.

### 4. Evaluation Metrics
Evaluated model performance using standard regression evaluation metrics:
* **Mean Squared Error (MSE):** Measures the average squared difference between estimated and actual values.
* **$R^2$ Score:** Indicates how well the model's predictions approximate the real-world data points.

---

## 🛠️ Tech Stack & Dependencies
* **Programming Language:** Python
* **Environment:** Google Colab
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 🚀 How to Run the Project
1. Open **Google Colab**.
2. Run the automated dataset download script to fetch `IMDB-Movie-Data.csv`.
3. Execute the preprocessing, training, and evaluation cells sequentially.

# Fake Job Posting Detection

## 📌 Project Overview

**Fake Job Posting Detection** is a machine learning project designed to identify whether a job posting is **fraudulent or legitimate**.

The system analyzes both textual and structured job-related information. Textual attributes such as **job descriptions, requirements, company profiles, and other job details** are cleaned and transformed into numerical features using **TF-IDF**.

Multiple machine learning classification algorithms are then trained and compared to identify a suitable model for detecting fraudulent job postings.

---

## 🎯 Objectives

* Identify fraudulent and legitimate job postings.
* Explore and understand the job posting dataset.
* Handle missing values and duplicate records.
* Clean and preprocess textual data.
* Select useful features for prediction.
* Convert text into numerical features using **TF-IDF**.
* Train multiple machine learning classification models.
* Compare model performance using multiple evaluation metrics.
* Perform hyperparameter tuning to improve model performance.
* Develop a prediction system for classifying unseen job postings.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning
* **Jupyter Notebook / Google Colab**

---

## 🤖 Machine Learning Models

The project uses multiple classification algorithms:

### 1. Logistic Regression

Used as one of the main classification algorithms for distinguishing between fraudulent and legitimate job postings.

### 2. Naive Bayes

A probabilistic classification algorithm that is particularly useful for text classification problems.

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Missing Value Handling
   ↓
Duplicate Removal
   ↓
Exploratory Data Analysis
   ↓
Text Cleaning
   ↓
Feature Selection
   ↓
Text Feature Combination
   ↓
Train-Test Split
   ↓
TF-IDF Vectorization
   ↓
Model Training
   ↓
Logistic Regression
   ↓
Naive Bayes
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Hyperparameter Tuning
   ↓
Best Model Selection
   ↓
New Job Posting Prediction
```

---

## 📊 Data Preprocessing

The dataset is first explored to understand its structure and identify missing values and other data-quality issues.

The preprocessing steps include:

1. Checking dataset dimensions.
2. Examining column names and data types.
3. Identifying missing values.
4. Handling missing textual values.
5. Removing duplicate records.
6. Cleaning textual information.
7. Combining relevant text features.
8. Splitting the dataset into training and testing sets.

---

## 📝 Text Preprocessing

Important textual attributes such as:

* Job title
* Company profile
* Job description
* Requirements
* Benefits

are combined and cleaned.

The text-cleaning process includes:

* Converting text to lowercase
* Removing URLs
* Removing HTML tags
* Removing punctuation
* Removing unnecessary spaces

---

## 🔢 TF-IDF Feature Extraction

Machine learning models cannot directly process raw text.

Therefore, **TF-IDF (Term Frequency-Inverse Document Frequency)** is used to convert textual information into numerical feature vectors.

The resulting numerical representation is used as input for the classification models.

---

## 📈 Model Evaluation

The models are evaluated using multiple metrics rather than relying only on accuracy.

The evaluation metrics include:

* **Accuracy**
* **Precision**
* **Recall**
* **F1 Score**
* **ROC-AUC**
* **Confusion Matrix**

### Confusion Matrix

The confusion matrix helps identify:

* True Positives
* True Negatives
* False Positives
* False Negatives

---

## 📊 Model Comparison

The performance of Logistic Regression and Naive Bayes is compared using the evaluation metrics.

The comparison helps determine which model is more suitable for detecting fraudulent job postings.

The final model is selected based on its overall performance and suitability for the problem rather than relying on a single metric.

---

## ⚙️ Hyperparameter Tuning

Hyperparameter tuning is performed to investigate whether different model parameter values can improve performance.

**GridSearchCV** can be used to test different parameter combinations and select the best configuration based on the chosen evaluation metric.

---

## 🔍 Prediction System

After training and selecting the final model, the system can accept a new, unseen job posting.

The new job posting is:

```text
New Job Posting
      ↓
Text Cleaning
      ↓
TF-IDF Transformation
      ↓
Trained ML Model
      ↓
Prediction
      ↓
Fraudulent / Legitimate
```

The system produces a classification indicating whether the job posting is likely to be **fraudulent** or **legitimate**.

---

## 📁 Project Structure

```text
fake-job-posting-detection/
│
├── Fake_Job_Posting_Detection.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

If the dataset is included in the repository:

```text
fake-job-posting-detection/
│
├── Fake_Job_Posting_Detection.ipynb
├── fake_job_postings.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/fake-job-posting-detection.git
```

### 2. Open the project

```bash
cd fake-job-posting-detection
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

```bash
jupyter notebook
```

Then open:

```text
Fake_Job_Posting_Detection.ipynb
```

Alternatively, the notebook can be run directly in **Google Colab**.

---

## 📦 Requirements

The main Python libraries used in this project are:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

## ⚠️ Limitations

The project has some limitations:

* The model depends on the quality and representativeness of the training dataset.
* New types of fraudulent job postings may not be detected accurately.
* Text-based models may not capture every real-world characteristic of a fraudulent posting.
* Predictions should be treated as an indication rather than absolute proof that a job posting is fraudulent.

---

## 🚀 Future Improvements

Possible improvements include:

* Testing additional machine learning algorithms.
* Using advanced NLP techniques.
* Applying deep learning or transformer-based models.
* Adding more structured job-posting features.
* Improving text preprocessing.
* Using larger and more diverse datasets.
* Developing a web-based interface for real-time predictions.

---

## 🎓 Project Purpose

This project demonstrates the application of **Machine Learning and Natural Language Processing techniques** to a real-world problem involving fraudulent online job postings.

It covers the complete machine learning workflow from **data preprocessing and feature extraction to model training, evaluation, comparison, tuning, and prediction**.

---

## 👨‍💻 Author

**Your Name**

GitHub: `https://github.com/YOUR-USERNAME`

---

## 📄 License

This project is created for **educational and academic purposes**.

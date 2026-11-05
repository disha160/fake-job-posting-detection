# Fake Job Posting Detection

## Project Overview
Fake Job Posting Detection is a Machine Learning project that identifies potentially fraudulent job advertisements by analyzing job-related textual information.

The system uses Natural Language Processing (NLP) and classification algorithms to distinguish between legitimate and fraudulent job postings.

## Dataset
- Dataset: Fake Job Postings (EMSCAD)
- Total records: 17,880
- Total original columns: 18
- Target column: `fraudulent`
  - `0` – Legitimate job posting
  - `1` – Fraudulent job posting

Dataset source: [Kaggle – Real or Fake Fake Job Posting Prediction](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction)

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Natural Language Processing (NLP)
- TF-IDF Vectorization

## Project Workflow
1. Dataset loading and exploration
2. Missing value handling and data cleaning
3. Text preprocessing
4. Exploratory Data Analysis (EDA)
5. TF-IDF text vectorization
6. Training and testing data split
7. Machine Learning model training
8. Model evaluation and comparison
9. Hyperparameter tuning
10. Fake job posting prediction system

## Machine Learning Algorithms
- Logistic Regression
- Multinomial Naive Bayes
- Random Forest
- Linear Support Vector Machine (SVM)

## Model Evaluation

The tuned Logistic Regression model achieved the following test results:

| Metric | Score |
|---|---:|
| Accuracy | 98.18% |
| Precision | 77.84% |
| Recall | 87.28% |
| F1 Score | 82.29% |

Best hyperparameters:
- C: 10
- Solver: liblinear

## Prediction System
The project includes a prediction function that accepts job title, company profile, description, requirements, and benefits.

It classifies the supplied posting as:
- Legitimate Job Posting
- Fraudulent Job Posting

## How to Run the Project

1. Clone this repository.
2. Install the required libraries.
3. Open the Jupyter Notebook.
4. Ensure the dataset CSV is in the same project directory.
5. Run the notebook cells in order.

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Limitations
- Predictions depend on the patterns present in the training dataset.
- The model may not identify every type of job scam.
- New and evolving fraud techniques may affect performance.
- Predictions should be reviewed before making employment decisions.

## Conclusion
This project demonstrates how Machine Learning and NLP techniques can help identify suspicious job advertisements and support safer online job searching.
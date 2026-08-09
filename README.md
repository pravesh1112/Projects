# 🎓 Chance of Admission for Higher Studies

A Machine Learning regression project that predicts the **chance of admission
to a graduate program** using academic performance, standardized test scores,
university rating, recommendation strength, SOP, CGPA, and research experience.

[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pravesh1112/Projects/blob/main/Chance_of_admission.ipynb)

---

## 📌 Project Overview

Graduate admissions can be competitive, and students often want an estimate
of their admission probability based on their academic profile.

This project uses **Linear Regression** to estimate the `Chance of Admit`
from the following applicant features:

- GRE Score
- TOEFL Score
- University Rating
- Statement of Purpose (SOP)
- Letter of Recommendation (LOR)
- Undergraduate CGPA
- Research Experience

The complete analysis is implemented in a Google Colab/Jupyter Notebook.

---

## 🎯 Objective

The objectives of this project are to:

1. Load and understand the admission dataset.
2. Perform basic data exploration and analysis.
3. Select relevant features for prediction.
4. Split the data into training and testing sets.
5. Train a Linear Regression model.
6. Generate predictions on unseen test data.
7. Evaluate the model using regression metrics.

---

## 📊 Dataset

The dataset contains **400 student records**.

| Feature | Description |
|---|---|
| GRE Score | Graduate Record Examination score |
| TOEFL Score | TOEFL examination score |
| University Rating | University rating from 1 to 5 |
| SOP | Statement of Purpose rating |
| LOR | Letter of Recommendation rating |
| CGPA | Undergraduate CGPA |
| Research | Research experience (0 = No, 1 = Yes) |
| Chance of Admit | Target variable representing admission probability |

The original notebook loads the dataset directly from the YBI Foundation
Dataset repository.

Dataset source:

https://github.com/YBIFoundation/Dataset/blob/main/Admission%20Chance.csv

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

---

## 🔍 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Inspection
   ↓
Exploratory Analysis
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Linear Regression
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 🤖 Machine Learning Model

### Linear Regression

The project uses `LinearRegression` from Scikit-learn.

The model learns the relationship between the selected applicant features
and the target variable `Chance of Admit`.

The notebook uses the following seven predictive features:

```text
GRE Score
TOEFL Score
University Rating
SOP
LOR
CGPA
Research
```

The `Serial No` column is treated as an identifier and is not used for
prediction.

---

## 📈 Model Evaluation

The current notebook reports the following results on its test set:

| Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 0.04400 |
| Mean Absolute Percentage Error (MAPE) | 0.07575 |
| Mean Squared Error (MSE) | 0.00404 |

These values are based on the current notebook run and can change if the
train/test split or model configuration is changed.

---

## 🚀 How to Run

### Google Colab

1. Open the notebook using the **Open in Google Colab** button above.
2. Run the cells from top to bottom.
3. The dataset is loaded from its online source.
4. Review the analysis, predictions, and evaluation metrics.

### Run Locally

Clone the repository:

```bash
git clone https://github.com/pravesh1112/Projects.git
cd Projects
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start Jupyter:

```bash
jupyter notebook
```

Open:

```text
Chance_of_admission.ipynb
```

---

## 📁 Repository Structure

```text
Projects/
│
├── Chance_of_admission.ipynb
├── README.md
├── requirements.txt
├── DATASET.md
├── .gitignore
└── LICENSE
```

---

## 💡 Key Takeaways

The project demonstrates a complete beginner-to-intermediate Machine Learning
workflow:

- Working with a real-world tabular dataset
- Data inspection using Pandas
- Exploratory analysis
- Feature selection
- Train-test splitting
- Regression model training
- Generating predictions
- Evaluating regression performance

---

## 🔮 Future Improvements

Potential improvements for the project include:

- Compare Linear Regression with Random Forest, Decision Tree, and Gradient
  Boosting models.
- Add cross-validation.
- Perform hyperparameter tuning.
- Add an R² score and residual analysis.
- Create a reusable prediction function.
- Build an interactive Streamlit application.
- Deploy the prediction model as a web application.

---

## ⚠️ Disclaimer

The model provides an **estimated admission probability** based only on the
features available in the dataset. It should not be treated as a guaranteed
admission decision.

Actual admission decisions can depend on many additional factors such as
university-specific requirements, applicant pool, program competitiveness,
essays, recommendations, work experience, and other information not included
in this dataset.

---

## 👨‍💻 Author

**Pravesh Jangra**

GitHub: https://github.com/pravesh1112

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

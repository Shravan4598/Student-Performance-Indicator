
# Student Performance Indicator 🎓📊

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A Machine Learning project to analyze and predict student performance based on various socio-demographic and academic features.

## 🔗 GitHub Repository
**URL**: [Student-Performance-Indicator](https://github.com/Shravan4598/Student-Performance-Indicator)

## 📌 Problem Statement

This project aims to understand how a student's academic performance (test scores in math, reading, and writing) is influenced by other variables such as:

- Gender  
- Ethnicity  
- Parental level of education  
- Lunch type (standard or free/reduced)  
- Test preparation course (completed or not)

By analyzing these factors, we build a predictive model to identify patterns and determine what contributes most to better performance.

## 📂 Data Collection

- **Source**: [Kaggle Dataset - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)
- **Rows**: 1000  
- **Columns**: 8
  - `gender`
  - `race/ethnicity`
  - `parental level of education`
  - `lunch`
  - `test preparation course`
  - `math score`
  - `reading score`
  - `writing score`

## 🧠 ML Pipeline Overview

The project is structured with a proper machine learning pipeline, which includes:

1. **Data Ingestion**
2. **Data Transformation**
3. **Model Training**
4. **Model Evaluation**
5. **Model Deployment (Flask API)**

## 📊 Model Performance Summary

| Model                     | Dataset | RMSE   | MAE    | R² Score |
| ------------------------- | ------- | ------ | ------ | -------- |
| **Linear Regression**     | Train   | 5.3231 | 4.2667 | 0.8743   |
|                           | Test    | 5.3940 | 4.2148 | 0.8804   |
| **Lasso**                 | Train   | 6.5938 | 5.2063 | 0.8071   |
|                           | Test    | 6.5197 | 5.1579 | 0.8253   |
| **Ridge**                 | Train   | 5.3233 | 4.2650 | 0.8743   |
|                           | Test    | 5.3904 | 4.2111 | 0.8806   |
| **K-Neighbors Regressor** | Train   | 5.7092 | 4.5180 | 0.8554   |
|                           | Test    | 7.2516 | 5.6160 | 0.7839   |
| **Decision Tree**         | Train   | 0.2795 | 0.0187 | 0.9997   |
|                           | Test    | 7.8537 | 6.2100 | 0.7465   |
| **Random Forest**         | Train   | 2.3534 | 1.8581 | 0.9754   |
|                           | Test    | 6.0532 | 4.6950 | 0.8494   |
| **XGBRegressor**          | Train   | 1.0073 | 0.6875 | 0.9955   |
|                           | Test    | 6.4733 | 5.0577 | 0.8278   |
| **CatBoost Regressor**    | Train   | 3.0427 | 2.4054 | 0.9589   |
|                           | Test    | 6.0086 | 4.6125 | 0.8516   |
| **AdaBoost Regressor**    | Train   | 5.7647 | 4.7161 | 0.8526   |
|                           | Test    | 6.1219 | 4.7561 | 0.8460   |

## 🚀 Technologies Used

- Python 🐍  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn  
- Flask 🌐  
- HTML/CSS (for front-end)  
- AWS Elastic Beanstalk (for deployment)

## 🗂️ Project Structure

```bash
Student-Performance-Indicator/
│
├── app.py                      # Flask application
├── requirements.txt            # Python dependencies
├── templates/
│   └── home.html               # Web UI for predictions
├── static/
│   └── (optional CSS/images)   # Static files (if used)
├── src/
│   ├── components/             # Data ingestion, transformation, model trainer, etc.
│   ├── pipeline/               # End-to-end pipeline scripts
│   ├── utils.py                # Utility functions
│   └── logger.py, exception.py # Logging and error handling
├── artifacts/                  # Saved models and intermediate files
└── README.md                   # Project documentation
````

## 🧪 How to Run the Project Locally

```bash
# 1. Clone the repository
git clone https://github.com/Shravan4598/Student-Performance-Indicator.git
cd Student-Performance-Indicator

# 2. Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the Flask app
python app.py
```

* Visit the **homepage** at: [http://localhost:5000](http://localhost:5000)
* Visit the **prediction page** directly at: [http://localhost:5000/predictdata](http://localhost:5000/predictdata)

## 🌍 Deployment

* The project can be deployed on **AWS Elastic Beanstalk** using `application.py` and the `WSGIPath` configuration.
* Docker and requirements-based packaging can be used for container-based deployment.

## 🙌 Contributions

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

*Made with ❤️ by Shravan Kumar Pandey*

```

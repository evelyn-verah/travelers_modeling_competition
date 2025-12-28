
# Travelers Insurance Predictive Analytics
Forecasting Policyholder Call Behavior Using Machine Learning

## Project Overview
This project builds a machine learning solution to forecast how many times a policyholder will contact Travelers call centers. 
Accurate forecasting helps reduce operational cost, improve staffing efficiency, and enhance customer support experiences.

This repository is based on the Travelers Insurance Case Competition project.

---

## Business Objective
Travelers faces fluctuating call center volumes, making staffing and cost management difficult. 
This analytics solution enables:
- Better resource allocation
- Reduced operational cost
- Improved policyholder experience

---

## Dataset Summary
Dataset consisted of ~80,000 policyholder records with 20 features. 
Key feature categories:
- Prior call history
- Premium and financial indicators
- Household policy stats
- Geographic segmentation

Target variable: **Number of Calls Policyholder Will Make**

---

## Modeling Approach
We evaluated multiple models including:
- KNN Regressor
- Random Forest
- LightGBM
- Lasso Regression

Primary metric: **Gini Index**

Final Selected Model: **KNN**
 Strong performance  
 Highly interpretable  
 Business friendly

---

## Results Summary
| Model | Score |
|--------|--------|
| KNN | 0.24650 |
| Random Forest | 0.24549 |
| LightGBM | 0.24890 |

**KNN selected** due to best combination of performance + interpretability.

---

## Repository Structure
```
travelers-predictive-analytics/
│
├── data/
│   ├── sample_policy_data.csv
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_modeling.ipynb
│
├── src/
│   ├── preprocess.py
│   ├── model_training.py
│   ├── evaluate.py
│
├── results/
│   ├── model_results.json
│
├── requirements.txt
└── README.md
```

---

## Installation
```
pip install -r requirements.txt
```

---

## Run Model
```
python src/model_training.py
```

---

## Business Impact
- Enables proactive staffing decisions
- Supports financial planning
- Helps maintain strong customer experience

---

## Data Confidentiality Notice
For confidentiality reasons, the public version of this repository uses a **synthetic dataset** that closely mimics the structure, schema, and statistical behavior of the original Travelers Insurance dataset used in the competition. 

However:
- **The modeling pipeline**
- **Feature engineering steps**
- **Evaluation methodology**
- **Business context and findings**

are all faithfully preserved from the real project work.


## Author
Everlyn Musembi

# Student Performance Big Data Analytics Pipeline
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![Status](https://img.shields.io/badge/status-complete-green)

## Summary
A modular Big Data analytics pipeline built to convert raw educational data into 
actionable academic interventions. Developed as part of CSCE 5300 - Introduction 
to Big Data and Data Science at the University of North Texas.

This pipeline combines MapReduce simulation, supervised machine learning, 
collaborative filtering, and NLP sentiment analysis into a unified visual 
analytics dashboard.

## Key Results
| Module | Method | Result |
|---|---|---|
| Predictive Modeling | Gradient Boosting | 88% accuracy, F1: 0.87 |
| Predictive Modeling | Random Forest | 87% accuracy, F1: 0.86 |
| Recommendation Engine | Collaborative Filtering (Cosine Similarity) | Precision@5: 0.82 |
| Sentiment Analysis | VADER | Polarity gap: 0.747 |

## Pipeline Modules

### 1. MapReduce Simulation
Processes 1,200 student records using a MapReduce paradigm to aggregate 
performance by subject and identify at-risk students at scale.

### 2. Predictive Modeling — Early Warning System
Trains and compares three classifiers (Gradient Boosting, Random Forest, 
Logistic Regression) on five features to detect at-risk students early.

### 3. Recommendation Engine
User-based Collaborative Filtering using Cosine Similarity on a 
200-student × 12-course interaction matrix to suggest personalized 
academic resources.

### 4. Sentiment Analysis
VADER-based NLP analysis of student free-text feedback, producing a 
quantifiable Engagement Index correlated with academic performance.

## Tech Stack
- **Data Processing:** Python, Pandas, NumPy, MapReduce simulation
- **Machine Learning:** Scikit-learn (Random Forest, Gradient Boosting, Logistic Regression)
- **NLP:** VADER (vaderSentiment)
- **Recommendation:** Cosine Similarity (Sklearn)
- **Visualization:** Matplotlib, Seaborn

## Dataset
Synthetic dataset of 1,200 student records across 5 subjects and 12 courses, 
generated programmatically within the notebook. Features include attendance 
percentage, midterm score, quiz average, assignment score, forum posts, 
final score, label, and free-text feedback.

## Repository Structure
- `notebooks/` — Main Jupyter notebook with full pipeline
- `report/` — Final project report
- `presentation/` — Project presentation slides
- `graphs/` — Generated visualization outputs

## Reference
Manoharan et al. (2025). *Big data and analytics in education: Leveraging 
data to improve student performance.* IEEE WorldSUAS. 
DOI: 10.1109/WorldSUAS66815.2025.1119913

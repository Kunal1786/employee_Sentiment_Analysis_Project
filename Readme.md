# Employee Sentiment Analysis

## Project Overview

This project analyzes an unlabeled set of employee emails and assigns sentiment
(Positive, Negative, Neutral), then aggregates results to:

- Explore data structure and sentiment distribution (EDA)
- Compute monthly sentiment scores per employee (sender)
- Rank employees by sentiment score
- Identify potential flight risk employees (4+ negative emails in any rolling 30-day window)
- (Optional) Explore simple linear-model relationships between text features and sentiment scores

All code is implemented in **Python** using **Jupyter Notebook**.

---

## Files in this Repository

- `Employee_Sentiment_Analysis.ipynb`  
  Main notebook that:
  - Loads `data/test.csv`
  - Cleans and preprocesses text
  - Applies sentiment scoring (VADER/TextBlob)
  - Performs EDA and saves plots into `visualizations/`
  - Calculates monthly sentiment scores
  - Ranks employees by sentiment
  - Flags flight-risk employees
  - (Optional) includes a linear regression section – commented/adjusted because dataset has no numeric target by default.

- `data/test.csv`  
  Input dataset (emails: subject, body, date, from).

- `visualizations/`  
  Folder containing generated PNG plots:
  - `sentiment_label_distribution.png`
  - `message_length_distribution.png`
  - `sentiment_over_time.png`
  - `monthly_score_distribution.png`
  - `model_residuals.png` (if regression enabled)

- `README.md`  
  This file.

- `report.docx` *(you will create in Word and save in this folder)*  
  Detailed write-up of approach, findings, and screenshots.

---

## Setup Instructions

### 1. Clone or download the project

```bash
cd Desktop
# if from GitHub:
git clone <your_repo_url>.git
cd Employee_Sentiment_Analysis_Project

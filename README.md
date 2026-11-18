# Machine Learning project specification


## 1. Project Title

- Project title: ***Fake News Predictor***

## 2. Team Members

**Write:**

- Names: **Annie Kadiambu - Alexandre Fath**
- Initial responsibilities: **Study the dataset**

## 3. Context and Motivation

- Application context: **Cybersecurity, fact-checking**
- Motivation: **Accurately determine whether published information is factual or misleading based on previously checked publications**
- Intended user or decision context, if relevant: **Independent journalists, Students, ARCOM**

## 4. Problem Statement

- Problem: **Knowing rapidly and with precision if a given statement is likely to be true or false**
- Main question: **Is a specific statement fake ?**
- Scope or boundary: **The project tackles only relatively short statements and not full articles**

## 5. Project Objectives

- Objective 1 and completion evidence: **Accuracy > 80%**
- Objective 2 and completion evidence: **Minimal execution time**

## 6. Dataset Description

Give a direct link to the dataset and identify its source organization, repository, or publication. Describe what one row represents, the approximate number of observations, available features, data types, and the target if one exists. Note known missing values, quality limitations, access steps, usage restrictions, and licensing. Explain why these data can address the stated problem. If the group will collect or generate data, describe the process and why it is feasible.

**Write:**

- Dataset name and direct link: `[URL]`
- Source: `[Organization, repository, or publication]`
- Unit of observation and approximate size: `[What does one row represent? How many rows?]`
- Features, data types, and target/output: `[What is available?]`
- Suitability and known limitations: `[Why can this answer the question? What may be difficult?]`
- Access, license, or collection feasibility: `[What has the team checked?]`

## 7. Machine Learning Task

- Task: **Classification**
- Inputs: **Title, Text, Subject, Date**
- Target or expected output: **Boolean value (0=not fake / 1=fake)**
- Measurable goal: **Metrics such as accuracy precision and actual real-life predicition may determine how well the model behaves**

## 8. Baseline Strategy

- Baseline algorithm: **Logistic Classifier**
- Why it is appropriate: **It is a basic classification algorithm ans as such it qualifies as a decent baseline**
- How it will be compared with later approaches: **The metrics listed below will be used to compare the model with later entries**

## 9. Evaluation Strategy

- Split or validation plan: **Random splits with increasing distribution percentage for each split**
- Metrics: **Accuracy, precision, recall, F1-score**
- Fit boundary: `[Which steps learn from training data? How will choices be made?]`
- Evaluation limitations: **It is unclear whether the dataset is representative of the actual distribution of fake news in general and the model may as such adopt a bias towards one category**

## 10. Initial Work Plan

- First tasks and order: **Dataset exploration, cleaning, scaling, preprocessing, testing of different classifier models, conclusion**
- Responsibilities: **All tasks will be shared**
- Week 1 feasibility check: **Dataset exploration**
- Open questions: **The model may be eventually tested on real data for actual use**

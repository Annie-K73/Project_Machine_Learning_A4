# Machine Learning project specification


## 1. Project Title

- Project title: ***Fake News Predictor***

## 2. Team Members


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


- Dataset name and direct link: **Fake News Dataset (kaggle)** [https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset?select=True.csv]
- Source: Organization (University of Victoria)
- Unit of observation and approximate size: **1 row = 1 article associated to a label (fake or real). Training set : 40 000 observations ; Test set : 4 000 observations**
- Features, data types, and target/output: 
	|Features| index| title| text| subject| date| class (target)|
	|---|---|---|---|---|---|---|
	|Data types| int| string|string|string|object|string|
	
- Suitability and known limitations: **We have a large variety of observations coming from genuine and legitimate news sites, but the dataset is balanced (52% fake news - 48 % real news) which may not be representative of the journalistic spectruum.**
- Access, license, or collection feasibility: **CC BY-NC-SA 4.0 ; Attribution-NonCommercial-ShareAlike 4.0 International**

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

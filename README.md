# FIETS Language Model Evaluation & Data Cleaning Project (Python)

## Overview

This project demonstrates end-to-end data analysis in Python using a **noisy, real-world dataset**. The goal is to evaluate and compare the performance of three large language models (LMs) on the **MMLU (Massive Multitask Language Understanding)** benchmark, while dealing explicitly with inconsistent, incomplete, and biased data.

The analysis focuses on **data cleaning, exploratory data analysis (EDA), aggregation, statistical reasoning, and fair model comparison**, reflecting challenges commonly encountered in practical data analyst roles.

---

## Problem Context

The dataset contains multiple-choice question results from three language models across 57 academic subjects.
However, the raw outputs are **corrupted and inconsistent**, including:

* Answers embedded in text (e.g. `"Answer: B"`)
* Trailing spaces or punctuation
* Lower-case or uncertain answers
* Missing values
* Uneven subject coverage between models

The task is to clean these outputs, quantify model accuracy, identify dataset imbalance, and produce a **robust and defensible comparison**.

---

## What This Project Tests

### 1. Data Loading & Inspection

* Reading and inspecting multiple CSV files with `pandas`
* Verifying dataset sizes and structural consistency
* Manually validating raw data before automation

**Skills demonstrated:**
`pandas`, filesystem handling, exploratory inspection

---

### 2. Robust Data Cleaning

* Detecting and standardising inconsistent answer formats
* Handling missing, invalid, and uncertain responses explicitly
* Creating cleaned columns while preserving original data for traceability
* Applying string operations and custom cleaning logic at scale

**Skills demonstrated:**
String manipulation, defensive data cleaning, reproducible preprocessing

---

### 3. Feature Engineering & Scoring Logic

* Mapping model outputs to ground-truth answers
* Implementing flexible scoring logic (including treatment of “unsure” answers)
* Computing per-model accuracy metrics

**Skills demonstrated:**
Feature engineering, boolean logic, metric construction

---

### 4. Data Integration

* Performing inner joins across datasets using unique identifiers
* Combining model predictions with question metadata (subject, correct answer)

**Skills demonstrated:**
Relational joins, dataset alignment, integrity checks

---

### 5. Exploratory Data Analysis (EDA)

* Analysing accuracy distributions across models
* Investigating subject-level coverage differences
* Identifying structural bias caused by uneven sampling

**Skills demonstrated:**
EDA, grouping & aggregation, analytical reasoning

---

### 6. Dataset Bias Detection & Rebalancing

* Quantifying subject-level imbalance between models
* Designing and implementing a **custom rebalancing strategy**
* Iteratively removing excess samples to achieve fair comparison
* Recomputing accuracy on balanced data

**Skills demonstrated:**
Bias analysis, algorithmic thinking, fairness-aware evaluation

---

### 7. Statistical & Analytical Rigor

* Clear separation of raw vs processed data
* Justification of methodological choices
* Emphasis on robustness and generalisability over naïve accuracy

**Skills demonstrated:**
Critical thinking, statistical awareness, analytical communication

---

## Technologies Used

* **Python**
* **pandas** – data manipulation and analysis
* **NumPy** – numerical operations
* **Matplotlib** – exploratory visualisation
* **SciPy** – statistical testing


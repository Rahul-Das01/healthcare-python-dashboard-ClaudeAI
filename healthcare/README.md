# Synthetic Healthcare Dataset

A synthetic healthcare dataset built to mimic real-world patient admission records. It is designed for practising data cleaning, analysis, visualization, and machine learning in a healthcare context.

> **Note:** All data is entirely synthetic. It was generated with Python's [Faker](https://faker.readthedocs.io/) library and contains no real patient information, so it does not violate any privacy regulations.

---

## Table of Contents

- [Overview](#overview)
- [Motivation](#motivation)
- [Data Dictionary](#data-dictionary)
- [Usage Scenarios](#usage-scenarios)
- [Getting Started](#getting-started)
- [Acknowledgments](#acknowledgments)

---

## Overview

Healthcare data is often sensitive and restricted by privacy rules, which makes it hard to access for learning and experimentation. This dataset mirrors the structure and attributes commonly found in healthcare records, so analysts and students can work with realistic data without any privacy concerns.

Each row describes a patient, their admission, and the healthcare services provided.

## Motivation

The dataset was created to fill the gap in practical, diverse healthcare data for educational and research purposes. The goal is to encourage innovation, learning, and knowledge sharing in the healthcare analytics domain.

## Data Dictionary

| Column | Description |
|---|---|
| `Name` | Name of the patient associated with the record |
| `Age` | Age of the patient at admission, in years |
| `Gender` | Gender of the patient (`Male` or `Female`) |
| `Blood Type` | Patient's blood type (e.g., `A+`, `O-`) |
| `Medical Condition` | Primary diagnosis (e.g., `Diabetes`, `Hypertension`, `Asthma`) |
| `Date of Admission` | Date the patient was admitted to the facility |
| `Doctor` | Name of the doctor responsible for the patient's care |
| `Hospital` | Healthcare facility where the patient was admitted |
| `Insurance Provider` | Patient's insurer (`Aetna`, `Blue Cross`, `Cigna`, `UnitedHealthcare`, `Medicare`) |
| `Billing Amount` | Amount billed for services during the admission (float) |
| `Room Number` | Room where the patient was accommodated |
| `Admission Type` | Circumstances of admission (`Emergency`, `Elective`, `Urgent`) |
| `Discharge Date` | Date of discharge, based on the admission date plus a random number of days within a realistic range |
| `Medication` | Medication prescribed or administered (e.g., `Aspirin`, `Ibuprofen`, `Penicillin`, `Paracetamol`, `Lipitor`) |
| `Test Results` | Outcome of a medical test (`Normal`, `Abnormal`, `Inconclusive`) |

## Usage Scenarios

This dataset can be used for:

- Developing and testing healthcare predictive models
- Practising data cleaning, transformation, and analysis techniques
- Creating data visualizations to uncover healthcare trends
- Learning and teaching data science and machine learning concepts in a healthcare setting
- Solving a **multi-class classification problem** to predict `Test Results` (3 classes: Normal, Abnormal, Inconclusive)

## Getting Started

```python
import pandas as pd

df = pd.read_csv("healthcare_dataset.csv")

print(df.shape)
print(df.info())
print(df.head())
```

### Suggested first steps

1. Check for missing values and duplicate records
2. Standardize text columns (e.g., inconsistent capitalization in `Name`)
3. Convert `Date of Admission` and `Discharge Date` to datetime and compute length of stay
4. Explore billing by medical condition, insurance provider, and admission type

## Acknowledgments

This dataset is entirely synthetic. The author acknowledges the importance of healthcare data privacy and security, and hopes the dataset contributes to the advancement of data science and healthcare analytics. Feel free to explore, analyze, and share your findings with the Kaggle community.

**Image credit:** Image by BC Y from Pixabay

# Mood, Age, and Ethnicity-Based Recommender System

## Project Overview
This project implements a **personalized music recommender system** based on user **mood, age, and ethnicity**. Unlike traditional systems, it integrates **physiological signals** and **demographic information** to provide contextually relevant and accurate recommendations. The system analyzes mood using physiological datasets and combines it with age and ethnicity-related preferences to deliver music that resonates with the listener’s current state and background.

---

## Datasets
Due to size and privacy, the full datasets are not included. You can access them from the following sources:

- **WESAD** – Physiological data for mood analysis  
  [Kaggle Link](https://www.kaggle.com/datasets/mohamedasem318/wesad-full-dataset)

- **DAPPER** – Mood data (physiological and behavioral)  
  [Synapse Link](https://www.synapse.org/Synapse:syn22418021/files/)

- **Wearables Stress and Exercise Dataset** – Age-related physiological data  
  [PhysioNet Link](https://physionet.org/content/wearable-device-dataset/1.0.0/)

> **Note:** A small sample dataset is included to allow the notebook to run.

---

## Objective
- Predict **user mood** using physiological signals.  
- Incorporate **age-specific preferences** to personalize recommendations.  
- Incorporate **ethnicity-related signals** to improve cultural relevance.  
- Generate **personalized music recommendations** based on mood, age, and ethnicity.  
- Optimize system performance; improved accuracy from ~55% → 85–90% using ensemble and class-specific techniques.

---

## Approach

### 1. Data Preprocessing
- Handle missing values, normalize signals, and encode categorical variables.  
- Merge datasets to create unified user profiles.

### 2. Feature Engineering
- Extract key physiological features for mood prediction.  
- Engineer demographic features for age and ethnicity preferences.

### 3. Modeling
- Train models for **mood classification** using physiological data.  
- Combine predictions with **age and ethnicity classifiers** to generate final recommendations.  
- Use feature extraction and **SMOTE techniques** to improve accuracy and class-specific predictions.

### 4. Recommendation Generation
- Map predicted mood, age, and ethnicity to music preferences.  
- Fetch songs dynamically using **YouTube API**.

---

## Results / Insights
- Mood classification accuracy improved from **55% → 85–90%**.  
- Personalized music recommendations closely match user mood and demographics.  
- Combining **mood + age + ethnicity** significantly improves recommendation relevance compared to baseline models.

---

## Files in Repository
- `Mood_Age_Ethnicity_Recommender_System.ipynb` → Jupyter notebook with full code and analysis  
- `Mood_Age_Ethnicity_Recommender_System.html` → Output/visualizations  
- Data cleaning files

---

## Technologies Used
- **Python** (Pandas, NumPy, Scikit-learn, XGBoost, LightGBM)  
- **Jupyter Notebook**  
- **YouTube API** for music recommendations  
- **Data Visualization:** Matplotlib, Seaborn

---

## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/MohdKaif-byte/Mood-Age-and-Ethnicity-Based-Recommender-System.git

2.Install dependencies:

pip install -r requirements.txt

3.Open the notebook in Jupyter:

jupyter notebook Mood, Age, and Ethnicity Based Recommender System.ipynb



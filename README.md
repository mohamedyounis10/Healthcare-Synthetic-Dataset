# Healthcare (Synthetic) 🩺 — EDA 📊, ML Models 🤖 & Power BI Dashboard 📈

This repository contains a small **healthcare analytics** project using a **synthetic dataset** for educational purposes:
- 📒 A **Jupyter Notebook** for EDA, feature engineering, and baseline ML modeling
- 📈 A **Power BI dashboard** (`.pbix`) with supporting images

> ⚠️ **Note**: The dataset is **synthetic** (not real patient data). Model accuracy around ~30% is expected due to noise and class overlap.

---

## Table of Contents 🧭

- [Project Structure](#project-structure-)
- [Overview](#overview-)
- [Dataset](#dataset-)
- [Notebook](#notebook-)
  - [Steps](#steps-)
  - [Models](#models-)
  - [Results](#results-)
- [Power BI Dashboard](#power-bi-dashboard-)
- [Getting Started](#getting-started-)
  - [Requirements](#requirements-)
  - [Run the Notebook](#run-the-notebook-)
- [Notes & Limitations](#notes--limitations-)
- [HTML Header Template](#html-header-template-)
- [Author](#author-)
- [Acknowledgments](#acknowledgments-)
- [License](#license-)

---

## Project Structure 🗂️

```text
Healthcare/
├─ Dataset/
│  └─ healthcare_dataset.csv
├─ Dashboard/
│  ├─ Healthcare.pbix
│  ├─ doctors.png
│  └─ istockphoto.png
├─ docs/
│  └─ header.html
└─ notebook.ipynb
```

---

## Overview ✨

The goal of this project is to practice:
- 🔎 Exploratory Data Analysis (EDA)
- 🧩 Feature engineering (e.g., stay duration)
- 🧪 Training and evaluating baseline classifiers
- 📊 Building a simple BI dashboard (Power BI)

---

## Dataset 📦

Location: `Dataset/healthcare_dataset.csv`

Key columns (before preprocessing):
- 🧑‍🤝‍🧑 Demographics: Age, Gender, Blood Type
- 🏥 Visit details: Date of Admission, Discharge Date, Admission Type
- 💳 Financial: Billing Amount, Insurance Provider
- 💊 Medical: Medical Condition, Medication
- 🎯 Target: **Test Results** (Normal / Abnormal / Inconclusive)

---

## Notebook 📒

File: `notebook.ipynb`

### Steps 🧭

1. Load data from `Dataset/healthcare_dataset.csv`
2. EDA (info/describe, univariate & bivariate visualizations)
3. Cleaning (drop a few non-essential columns, parse dates)
4. Feature engineering (e.g., **Stay Duration**)
5. Encoding categorical columns + scaling numerical features
6. Train/test split + modeling + evaluation

### Models 🤖

- Logistic Regression (balanced class weights)
- Random Forest
- SVM (RBF kernel)

### Results ✅

Accuracy is around **0.33** (± a bit by model), which is reasonable for a **synthetic** dataset with weak/ noisy relationships.

---

## Power BI Dashboard 📈

Folder: `Dashboard/`

- `Healthcare.pbix`: Power BI report
- `doctors.png`, `istockphoto.png`: images used in the dashboard

Open the `.pbix` file using **Power BI Desktop**.

What you can do with the dashboard:
- 📌 Explore key distributions (e.g., demographics, admission types, medical conditions)
- 💳 Review billing/insurance breakdowns
- 🔎 Slice & filter visuals for quick insights
  
<img width="1290" height="724" alt="Screenshot 2026-02-04 090056" src="https://github.com/user-attachments/assets/de569998-d27e-4f53-b611-bf77179efd11" />

---

## Getting Started 🚀

### Requirements 🧰

To run the notebook, you’ll typically need:
- Python 3.x
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

---

### Run the Notebook ▶️

1. Open `notebook.ipynb` in Jupyter / VS Code.
2. Run cells top-to-bottom.

---

## Notes & Limitations 📝

- The dataset is **synthetic** and intended for practice, not clinical insights.
- Don’t over-optimize accuracy on synthetic/noisy labels; focus on workflow and interpretation.

---

## HTML Header Template 🧩

File: `docs/header.html`

- A simple, reusable **HTML header** (brand + navigation) with clean CSS.
- You can use it in a static website or GitHub Pages.

---

## Author ✍️

- Name: **Mohamed Younis**

---

## Acknowledgments 🙏

- **Internship 🏢**: [Uneeq Interns](https://www.linkedin.com/company/uneeq-interns/)

---

## License 📄

Add a license that matches how you want others to use your work (e.g., MIT).
If you tell me your preference, I can add the `LICENSE` file too.




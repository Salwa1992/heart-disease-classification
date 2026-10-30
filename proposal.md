# Project Proposal: Heart Disease Risk Classification

## 1. Research Question
Can we accurately classify whether a patient has a high risk of heart disease based on clinical metrics like age, cholesterol, maximum heart rate, and blood pressure? Which clinical metric stands out as the strongest linear predictor of heart disease presence?

## 2. Dataset Details
* **Dataset Name:** Heart Disease Dataset (Cleveland Cohort)
* **Source:** UCI Machine Learning Repository Link
* **Description:** This dataset contains 303 individual patient records across 14 clinical features. Features include patient demographics (age, sex), pain profile metrics (chest pain type), physiological rest data (resting blood pressure, serum cholesterol, fasting blood sugar, resting electrocardiographic results), and stress-test benchmarks (maximum heart rate achieved, exercise-induced angina, ST depression). The target label indicates the presence or absence of heart disease.

## 3. Two-Source Scan of Existing Work
* **Source 1:** *Detrano, R. et al. (1989). "International application of a new probability algorithm for the development of coronary artery disease." American Journal of Cardiology.*
  * **Takeaway:** This foundational paper shows that logistic regression models using age, sex, chest pain type, and ST segment abnormalities achieve an 77% accuracy rate. It confirms that exercise-induced metrics provide higher classification signal than resting metrics alone.
* **Source 2:** *Al-Mallah, M. et al. (2018). "Machine Learning in Cardiovascular Medicine: A Comprehensive Review." Progress in Cardiovascular Diseases.*
  * **Takeaway:** This source highlights the impact of data preprocessing on tree-based models versus linear models. It emphasizes that normalizing skewed clinical data (like cholesterol levels) drastically improves convergence rates during binary classification optimization steps.

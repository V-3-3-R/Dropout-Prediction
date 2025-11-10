# 🎓 JEE Dropout Prediction: Machine Learning Models for Identifying At-Risk Students

**Language:** Python  
**Libraries:** scikit-learn, pandas, seaborn, matplotlib  
**License:** MIT  

---

## 🧠 Overview

This project develops **machine learning models** to predict student dropout risks in **Joint Entrance Examination (JEE)** preparation programs after Class 12.  
Using a **simulated dataset**, we train and compare three classifiers:

- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting**

The goal is to identify key factors contributing to dropouts — such as **academic scores**, **study habits**, **family background**, and **mental health indicators** — and provide educators and institutes with an **early warning system** to support at-risk students.

---

## ✨ Key Features

- **Data Preprocessing:** Handles categorical encoding (one-hot) and numerical scaling.  
- **Model Comparison:** Evaluates accuracy, precision, recall, F1-score, and confusion matrices.  
- **Feature Importance:** Analyzes top predictors using tree-based models.  
- **Visualizations:** Bar charts, box plots, stacked bars, and heatmaps for insights.  
- **Reproducible:** Runs easily in **Jupyter Notebook** or as a **Python script**.

---

## 🗂️ Dataset

The project uses the **`JEE_Dropout_After_Class_12.csv`** dataset — a simulated collection of **5,000 student records** with **15 features**.  
It includes:

- **Academic metrics:** JEE scores, Class 12 percentage  
- **Socioeconomic factors:** Family income, parental education  
- **Behavioral indicators:** Daily study hours, mental health issues  

🎯 **Target variable:** `dropout`  
- `1` → Dropped out  
- `0` → Continued  

---

### 📥 Downloading the Dataset

1. Visit the **[Kaggle Dataset Page](https://www.kaggle.com/)**.  
2. Sign in or create a free account.  
3. Click **Download** (~377 KB ZIP).  
4. Extract and place `JEE_Dropout_After_Class_12.csv` in your project root directory.

> Note: The dataset is synthetic but realistic, designed to mimic real-world JEE preparation scenarios in India.

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/jee-dropout-prediction.git
cd jee-dropout-prediction
```

# Create and activate a virtual environment (recommended):
```bash
python -m venv venv
```
# On macOS/Linux
```bash
source venv/bin/activate
```
# On Windows
```bash
venv\Scripts\activate
```
# Install dependencies:
```bash
pip install -r requirements.txt
```
# Or install manually:
```bash
pip install pandas scikit-learn seaborn matplotlib numpy
```

# Requirements.txt
- pandas>=1.5.0
- scikit-learn>=1.2.0
- seaborn>=0.12.0
- matplotlib>=3.6.0
- numpy>=1.24.0

# 🚀 Usage
▶️ Running the Python Script
Execute the main script to load data, train models, evaluate performance, and generate plots:
python bda_rp.py

This will:
- Display data overview and splits
- Train and compare the three models
- Print performance metrics (e.g., F1-scores)
- Save visualizations as .png files (e.g., dropout_count_bar_chart.png)

# 💻 Running the Jupyter Notebook
For interactive exploration:
- ```bash
  jupyter notebook
  ```
- Then open DROPOUT2.ipynb and run all cells.

# 📊 Expected Output
| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | ~0.82    | ~0.80     | ~0.78  | ~0.79    |
| Random Forest       | ~0.88    | ~0.87     | ~0.85  | ~0.86    |
| Gradient Boosting   | ~0.90    | ~0.89     | ~0.88  | ~0.88    |

Metrics are based on an 80/20 stratified train-test split (random_state=42).
Dropout ratio ≈ 0.25 in both sets.

# 🌟 Top 5 Features (from Gradient Boosting)
| Rank | Feature Name               | Importance |
| ---- | -------------------------- | ---------- |
| 1️⃣  | `mock_test_score_avg`      | 0.25       |
| 2️⃣  | `daily_study_hours`        | 0.18       |
| 3️⃣  | `mental_health_issues_Yes` | 0.12       |
| 4️⃣  | `jee_advanced_score`       | 0.10       |
| 5️⃣  | `family_income_Low`        | 0.08       |

# 🤝 Contributing
Contributions are welcome!
To contribute:
# 1. Fork the repo
# 2. Create a feature branch
git checkout -b feature/amazing-feature
# 3. Commit your changes
git commit -m 'Add amazing feature'
# 4. Push to the branch
git push origin feature/amazing-feature
Then, open a Pull Request 🚀
Report any issues via GitHub Issues.

🙌 Acknowledgments

Dataset: Kaggle — Simulated Dataset: JEE Dropout After Class 12 by Jayaantanaath.
Tools: scikit-learn, pandas, seaborn, matplotlib.
Purpose: To promote data-driven educational interventions and reduce dropout rates in competitive exam preparation.

# 💡 Built with ❤️ for educational data science research and student success prediction.

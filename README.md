# 🏏 Predictive Analysis in Cricket

A machine learning project that predicts cricket match outcomes, player performance, and innings scores using multiple ML models.

---

## 📌 Project Overview

This project analyzes ODI cricket data to:
- Predict **match results** (Win/Loss)
- Predict **runs scored** by batsmen
- Predict **second innings score** from first innings data
- Identify **top-performing players and features**

---

## 📁 Project Structure

```
predictive_analysis_in_cricket/
│
├── data/
│   ├── Batsman_Data.csv
│   ├── Bowler_data.csv
│   └── Sorted_ODI_Match_Totals.csv
│
├── notebooks/
│   └── predictive_analysis_in_cricket.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── eda.py
│   ├── model_random_forest.py
│   ├── model_linear_regression.py
│   ├── model_neural_network.py
│   ├── model_svm.py
│   ├── model_decision_tree.py
│   └── model_xgboost.py
│
├── outputs/
│   └── high_accuracy_model.h5
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📊 Datasets Required

| File | Description |
|------|-------------|
| `Batsman_Data.csv` | Batting stats: Runs, BF, SR, 4s, 6s, etc. |
| `Bowler_data.csv` | Bowling stats: Overs, Wkts, Econ, Ave, etc. |
| `Sorted_ODI_Match_Totals.csv` | Match totals: Score, Target, Result, etc. |

Place all CSV files in the `data/` folder before running.

---

## 🤖 Models Implemented

| Model | Task | Key Metric |
|-------|------|------------|
| Random Forest Regressor | Predict Score | R² Score, MSE |
| Random Forest Classifier | Predict Result | Accuracy |
| Linear Regression (RF-based) | Predict Runs | R² Score, MAE |
| Neural Network (TensorFlow/Keras) | Binary classification | Accuracy |
| Support Vector Machine (SVM) | Match outcome | Accuracy |
| Decision Tree Classifier | Match outcome | Accuracy |
| XGBoost Regressor | Second innings score | MAE, R² |

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/predictive_analysis_in_cricket.git
cd predictive_analysis_in_cricket
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate           # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Add your data files
Place the 3 CSV files inside the `data/` folder.

### 5. Run the notebook
```bash
jupyter notebook notebooks/predictive_analysis_in_cricket.ipynb
```

Or run individual scripts:
```bash
python src/data_preprocessing.py
python src/model_random_forest.py
```

---

## 📈 Key Results

- **Random Forest (Score Prediction):** High R² with low MSE
- **Neural Network:** ~50% accuracy on binary classification
- **XGBoost (Innings Prediction):** Low MAE, high R²
- **Decision Tree & SVM:** Used for match outcome classification

---

## 🛠️ Tech Stack

- **Language:** Python 3.8+
- **ML Libraries:** scikit-learn, TensorFlow/Keras, XGBoost
- **Data:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Google Colab / Jupyter Notebook

---

## 👤 Author

Mrudula Shenoy  
GitHub: [@StarryLuna-pixel](https://github.com/your-username)

---

## 📄 License

This project is licensed under the MIT License.

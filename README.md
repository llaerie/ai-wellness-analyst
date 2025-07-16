# 🌐 NEXHA: Next Health Analytics  
**Personal Health Optimization with Wearable Data**

NEXHA is a personalized AI wellness analyst that analyzes wearable data from devices like Fitbit to optimize your **energy**, **recovery**, **sleep**, and **daily performance**.

---

## 🧠 Project Goal  
> “What should I do daily to feel and perform my best?”

This project explores Arielle's 2025 Fitbit data to uncover the **top daily habits** that boost **Heart Rate Variability (HRV)** — a key indicator of recovery and nervous system health.

---

## 🚀 Key Features

- 📈 **Predictive Modeling**: Random Forest + Linear Regression to forecast HRV  
- 🧩 **Feature Attribution**: SHAP & Permutation Importance for interpretability  
- 🔍 **Correlation Analysis**: Understand physiological relationships (HRV, RHR, VO₂ Max, sleep)  
- 🧠 **AI Lifestyle Coaching**: Generates personalized wellness feedback  
- 📊 **Interactive Visualizations**: Correlation heatmaps, SHAP plots, decision trees  

---

## 📊 Data Used

| Variable                 | Description                                          |
|--------------------------|------------------------------------------------------|
| `AVG_HRV`               | 💓 Target: Heart Rate Variability during sleep       |
| `READINESS_SCORE`       | 🟢 Daily recovery indicator from Fitbit               |
| `VO2MAX`                | 🏃‍♀️ Cardiovascular fitness estimate                  |
| `RHR`                   | ❤️ Resting Heart Rate                                |
| `DEEP_SLEEP`            | 🌙 Minutes in deep sleep stage                       |
| `REVITALIZATION_SCORE` | 😌 Subjective sleep restoration score                |

---

## 🔬 Summary of Findings

| Rank | Driver                | Importance | Insight                                                                 |
|------|-----------------------|------------|-------------------------------------------------------------------------|
| 🥇   | `READINESS_SCORE`      | 0.68       | Strongest predictor of HRV. Reflects nervous system recovery.          |
| 🥈   | `VO2MAX`               | 0.45       | Aerobic fitness boosts parasympathetic resilience.                     |
| 🥉   | `RHR`                  | 0.17       | Lower RHR = higher HRV. Indicates better cardiovascular recovery.      |
| 4️⃣  | `DEEP_SLEEP`           | 0.03       | Slight influence, but not a primary driver.                            |
| 5️⃣  | `REVITALIZATION_SCORE`| 0.01       | Weak predictor — may be too holistic or noisy.                         |

**Model Performance:**  
- 📈 **R² = 0.77** (Linear Regression)  
- ✅ Accurately predicts HRV from 5 physiological metrics  
- 🧠 Learned biologically meaningful relationships (verified with SHAP & trees)

---

## 🧠 Personalized AI Coaching

> “Hi Arielle! Based on your data, here’s how to boost your recovery and performance 👇”

### ✅ Top Recommendations

| Priority | Action                                         | Why It Works                                       |
|----------|------------------------------------------------|----------------------------------------------------|
| ⭐⭐⭐     | Track and adapt workouts to readiness score     | Avoids overtraining and improves HRV               |
| ⭐⭐      | Add 30–60 min low-intensity cardio 3–5×/week    | Boosts VO₂ Max and heart resilience                 |
| ⭐        | Set a consistent bedtime/wake time             | Lowers resting HR and supports overnight recovery  |

> 💡 *"If you follow this plan, you could boost your average HRV by 15–20% in 6–8 weeks — helping you feel more energized, calm, and resilient."*

---

## 🛠️ Tech Stack

- `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `statsmodels`
- `shap`, `permutation_importance`
- ML Models: Random Forest Regressor, OLS Linear Regression
- Optional: Streamlit or Flask for web app deployment

---

## 📈 Sample Visuals

- 🔥 Correlation heatmap
- 🧠 SHAP summary & beeswarm plots
- 📊 Predicted vs actual HRV scatter
- 🌳 Simplified decision tree logic

> These visuals explain what drives your recovery — not just predict it.

---

## 🔮 Future Work

- ✍️ Add journaling/mood/nutrition data for deeper context  
- ⏳ Forecast HRV trends with ARIMA or Prophet  
- 🌐 Deploy as a Streamlit or Flask app  

---

## 👩‍💻 About the Creator

This project was built by **Arielle Leong**, a pharmacology graduate and aspiring health data scientist. She's passionate about turning wearable data into actionable wellness feedback.

**NEXHA** is her vision to empower users with AI-driven health insights grounded in science and self-optimization.

---

## ✅ Want to Try NEXHA?

Want to run NEXHA on your own Fitbit or Apple Health data?

1. Export your `.csv` or `.json` from Fitbit
2. Clone the repo and run the notebook
3. Get personalized insights and predictions

📁 GitHub Repo: [github.com/llaerie](https://github.com/llaerie)  
📬 Contact: [linkedin.com/in/arielleleong](https://www.linkedin.com/in/arielleleong)

---

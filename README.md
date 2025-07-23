# 🚀 Startup Health Scoring Model

This project presents a scoring system that evaluates the overall health and potential of fictional startups based on various critical business metrics. It helps stakeholders like investors, incubators, and entrepreneurs identify strong startups and diagnose potential weaknesses.

---

## 📌 Project Summary

We analyzed a dataset of 100 fictional startups using six key business parameters. Each startup was assigned a health score ranging from 0 to 100 based on a weighted and normalized combination of these features.

**Key Results:**
- 📊 **Average Score:** 49.85  
- 🥇 **Highest Score:** 84.32 (Startup ID: `S059`)  
- 🧨 **Lowest Score:** 15.89 (Startup ID: `S023`)  
- 📈 **Score Range:** 15.89 – 84.32  

---

## 🎯 Features Used in Scoring

| Feature | Impact | Description | Weight |
|--------|--------|-------------|--------|
| Monthly Active Users | Positive | Reflects product traction | 25% |
| Team Experience | Positive | Average years of experience among founding team | 20% |
| Valuation (INR) | Positive | Indicative of market trust and growth | 15% |
| Market Size (USD) | Positive | Total addressable market | 15% |
| Burn Rate (INR) | Negative | Monthly cash outflow (lower is better) | 15% |
| Funds Raised (INR) | Positive | Total funding received | 10% |

- ✅ **Positive features** contribute directly to score.  
- ⚠️ **Negative feature** (Burn Rate) is scaled inversely.

---

## 🧮 Scoring Methodology

1. **Normalization**:  
   Each feature is scaled using **Min-Max normalization** to bring all values between 0 and 1.

2. **Weighting**:  
   Each normalized feature is multiplied by its assigned weight.

3. **Final Score**:  



---

## 📊 Visualizations Included

The notebook generates key insights and visuals to support the analysis:

- 📈 **Score Distribution** – Histogram of all startup scores  
- 🔥 **Top 10 Startups** – Bar chart of best performers  
- 🧪 **Feature Correlation Heatmap** – Understand how features relate  
- 💸 **Valuation vs Score** – Scatter plot showing investment vs quality  
- ⚖️ **Feature Weights** – Visual of each feature's importance

---

## 💡 Key Insights

- High scores are often driven by **strong traction (users)** and **experienced teams**.
- Startups with **low burn rates** and **large market size** tend to rank higher.
- A high valuation alone doesn't guarantee a high score—balanced metrics matter.

---

## 🛠 Tech Stack

- **Python** for analysis  
- **Pandas**, **NumPy** for data manipulation  
- **Scikit-learn** for normalization  
- **Matplotlib**, **Seaborn** for visualization  

---

## 📁 Outputs

- ✅ `startup_scores.csv`: Contains startup IDs and their corresponding scores  
- 📊 Plots and graphs: Generated inline in the notebook for quick insights  

---

## 🚧 Future Enhancements

- 🧠 Integrate ML to auto-learn feature weights  
- 🌐 Build a Flask or Streamlit web app for interactive scoring  
- 📊 Create dashboards using Plotly or Tableau  
- 🧾 Include sector-based scoring filters

---

## 📅 Submission Details

- 👨‍💻 **Submitted For**: ScaleDux AI Internship — Task 1  
- 📍 **Submission Date**: July 24, 2025  
- 📂 **Notebook**: `startup_health_scoring.ipynb`  
- 📝 **Report**: README + code + visuals

---

## 🙌 Acknowledgements

Special thanks to the ScaleDux AI team for the opportunity and support throughout this task.

---




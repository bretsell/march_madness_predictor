# 🏀 March Madness Predictor  
ECE 204 – Final Group Project  
University of Wisconsin–Madison  

---

## 📌 Project Overview  

This project analyzes historical NCAA Division I Men’s Basketball Tournament data to identify key statistical indicators of teams that make deep tournament runs and to build a predictive model for March Madness matchups.

Our primary goal was to:

- Identify trends and features that correlate with tournament success  
- Engineer meaningful matchup-level features  
- Train and evaluate a classification model to predict game winners  
- Apply insights to bracket-style predictions  

Rather than relying on intuition or seeding alone, this project uses data-driven modeling to evaluate what truly predicts tournament performance.

---

## 🎯 Motivation  

March Madness is famously unpredictable — but underlying performance metrics often reveal consistent patterns among successful teams.

We aimed to answer:

- Do offensive metrics matter more than defensive metrics?
- Is seeding as predictive as people think?
- What statistical gaps between teams drive wins?
- Can we systematically predict matchup outcomes?

This project combines statistical analysis, feature engineering, and machine learning to approach bracket prediction analytically.

---

## 📂 Repository Structure  

```
📁 data/
    Raw and cleaned datasets

📓 preprocessing.ipynb
    Data cleaning, merging, feature engineering

📓 final_model.ipynb
    Model training, evaluation, and prediction analysis

README.md
```

---

## 🧹 Preprocessing Notebook  

The **Preprocessing Notebook** handles:

- Cleaning historical tournament and team statistics data
- Handling missing values and formatting inconsistencies
- Creating matchup-level features
- Generating statistical differentials between teams
- Encoding categorical variables (e.g., seeds, conferences)

### Key Feature Engineering Steps

- Seed difference (Team A – Team B)
- Offensive efficiency gap
- Defensive efficiency gap
- Turnover margin difference
- Rebounding margin difference
- Win percentage differential
- Advanced statistics normalization

Each row in the processed dataset represents a single tournament matchup with a binary outcome label.

---

## 🤖 Final Model Notebook  

The **Final Notebook** includes:

- Model selection and training
- Train/test split evaluation
- Cross-validation
- Feature importance analysis
- Prediction outputs for bracket simulation

### Models Explored

- Logistic Regression  
- Decision Trees  
- Random Forest  

The final selected model was chosen based on predictive accuracy, interpretability, and stability across validation folds.

---

## 📊 Evaluation Metrics  

We evaluated performance using:

- Accuracy
- Confusion matrix
- Cross-validation score
- Feature importance ranking

Given the volatility of tournament play, we focused on consistent predictive patterns rather than overfitting to specific seasons.

---

## 🔍 Key Insights  

- Seed difference remains predictive but is not sufficient alone.
- Defensive metrics and efficiency margins strongly influence deep runs.
- Balanced teams (strong offense + strong defense) outperform extreme single-strength teams.
- Turnover margin and rebounding differential often separate close matchups.
- Advanced efficiency metrics outperform raw counting stats.

---

## 🛠 Technologies Used  

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## 🚀 How to Run  

1. Clone the repository:
   ```bash
   git clone <repo-link>
   cd march-madness-predictor
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

3. Run notebooks in order:
   - `preprocessing.ipynb`
   - `final_model.ipynb`

---

## 📈 Future Improvements  

If expanded beyond this course project, we would:

- Incorporate player-level metrics
- Use Elo ratings
- Add momentum features (last 10 games performance)
- Include betting spread comparisons
- Explore gradient boosting models (XGBoost, LightGBM)
- Simulate full bracket Monte Carlo predictions

---

## 👥 Team Contribution  

This was a collaborative group project for ECE 204. Responsibilities were divided across:

- Data cleaning and preprocessing  
- Feature engineering  
- Model development and validation  
- Documentation and interpretation  

---

## 🏆 Final Takeaway  

March Madness will always have upsets — but data reveals patterns.

By combining statistical reasoning with machine learning, we built a structured, reproducible framework for evaluating tournament matchups beyond intuition.

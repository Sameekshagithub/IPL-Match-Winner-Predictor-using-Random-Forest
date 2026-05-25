# IPL-Match-Winner-Predictor-using-Random-Forest
```markdown

An end-to-end Machine Learning project that predicts IPL match winners using a Random Forest Classifier, complete with a Flask web application featuring a professional dark-themed dashboard.

```
## 📁 Project Structure

IPL_Match_Prediction.ipynb   ← Single notebook (everything inside)
ipl_rf_model.pkl             ← Auto-generated after training
```

---

## 🚀 Features

- ✅ Synthetic IPL dataset (2,000 matches) with realistic match logic
- ✅ Exploratory Data Analysis with 6 matplotlib/seaborn plots
- ✅ Feature engineering (RRR, CRR, balls remaining, etc.)
- ✅ Random Forest Classifier (200 estimators)
- ✅ Accuracy score, classification report & confusion matrix
- ✅ Feature importance visualization
- ✅ Model saved with Pickle
- ✅ Flask web app on port 5001
- ✅ Dark glassmorphism UI with animated predict button

---

## 🛠️ Installation

```bash
pip install pandas numpy scikit-learn flask matplotlib seaborn
```

---

## ▶️ How to Run

1. Open `IPL_Match_Prediction.ipynb` in Jupyter Notebook or JupyterLab
2. Run all cells top to bottom (**Cell → Run All**)
3. When Cell 9 starts, open your browser at:

```
http://localhost:5001
```

---

## 📊 Model Details

| Parameter | Value |
|-----------|-------|
| Algorithm | Random Forest Classifier |
| Estimators | 200 |
| Max Depth | 15 |
| Test Split | 20% |
| Features | 16 |

### Features Used

| Feature | Description |
|---------|-------------|
| `batting_team` | Team currently batting |
| `bowling_team` | Team currently bowling |
| `city` | Match venue city |
| `target` | First innings target |
| `score` | Current score |
| `overs` | Overs completed |
| `wickets` | Wickets lost |
| `toss_winner` | Team that won the toss |
| `toss_decision` | Bat or Field |
| `runs_needed` | Runs left to win |
| `balls_remaining` | Balls left in innings |
| `wickets_remaining` | Wickets in hand |
| `current_run_rate` | CRR (score / overs) |
| `required_run_rate` | RRR (runs needed per over) |
| `run_rate_diff` | RRR − CRR |
| `toss_match_bat` | Toss winner chose to bat |

---

## 🌐 Web App Inputs

| Field | Description |
|-------|-------------|
| Batting Team | Team currently chasing |
| Bowling Team | Team that bowled first |
| City | Venue of the match |
| Target Score | First innings total + 1 |
| Current Score | Runs scored so far |
| Overs Completed | e.g. 13.4 |
| Wickets Out | Wickets fallen (0–9) |
| Toss Winner | Team that won the toss |
| Toss Decision | Bat / Field |

### Output

- 🏆 Predicted Winner
- 📈 Win Probability %
- 📉 Lose Probability %
- 📋 Match Summary (RRR, CRR, Balls Left, Wickets Remaining)

---

## 📸 Notebook Steps

| Step | Description |
|------|-------------|
| 1 | Library Imports |
| 2 | Dataset Generation |
| 3 | Exploratory Data Analysis |
| 4 | Feature Engineering & Preprocessing |
| 5 | Random Forest Model Training |
| 6 | Model Evaluation |
| 7 | Save Model with Pickle |
| 8 | Sample Prediction Demo |
| 9 | Flask Web App (port 5001) |

---

## 🧪 Sample Prediction

```
Batting Team  : Mumbai Indians
Bowling Team  : Chennai Super Kings
City          : Mumbai
Target        : 180
Current Score : 120 / 4
Overs         : 14.0

→ Predicted Winner : Mumbai Indians
→ Win Probability  : 63.5%
→ Lose Probability : 36.5%
```

---

## 🏏 Supported Teams

- Mumbai Indians
- Chennai Super Kings
- Royal Challengers Bangalore
- Kolkata Knight Riders
- Delhi Capitals
- Rajasthan Royals
- Sunrisers Hyderabad
- Punjab Kings
- Gujarat Titans
- Lucknow Super Giants

---

## 📍 Supported Cities

Mumbai · Chennai · Bangalore · Kolkata · Delhi · Jaipur · Hyderabad · Chandigarh · Ahmedabad · Lucknow · Pune · Durban · Johannesburg · Cape Town

---

## 🔧 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10+ | Core language |
| scikit-learn | Random Forest, preprocessing |
| pandas / numpy | Data manipulation |
| matplotlib / seaborn | Visualization |
| Flask | Web server |
| pickle | Model serialization |
| Jupyter Notebook | Development environment |

---

## ⚠️ Notes

- The dataset is **synthetically generated** with realistic IPL-style logic. For real-world accuracy, replace Cell 2 with the Kaggle IPL dataset.
- The model pickle file (`ipl_rf_model.pkl`) is auto-created when you run the notebook — no manual setup needed.
- To stop the Flask server, press `Ctrl + C` in the Jupyter terminal.

---

*Built with ❤️ using Random Forest · scikit-learn · Flask*
```

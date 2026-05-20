# Fantasy Premier League AI Assistant

An AI-assisted Fantasy Premier League (FPL) decision support system that uses machine learning, analytics, and optimization techniques to recommend balanced FPL squads and predict player performance using live FPL data.

---

## Overview

This project was built to assist Fantasy Premier League players in making smarter transfer, captaincy, and squad selection decisions through data-driven analysis rather than intuition alone.

The system combines:

- Live FPL API data
- Machine learning models
- Statistical analysis
- Constraint-based optimization
- Automated preprocessing pipelines

Instead of generating unrealistic “perfect” teams, the assistant focuses on creating practical and balanced recommendations under real FPL constraints such as budget, formation rules, and player limits per club.

---

## Features

- Live player and fixture data collection using the official FPL API
- Data cleaning and preprocessing pipelines using Pandas and NumPy
- Machine learning models for player performance prediction
- Position-specific analysis for:
  - Goalkeepers
  - Defenders
  - Midfielders
  - Forwards
- Squad recommendation logic using linear programming (PuLP)
- Budget-aware and rule-based team generation
- Player ranking and comparison system
- Automated prediction workflow

---

## Tech Stack

### Languages & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- PuLP
- Requests

### Machine Learning
- Linear Regression
- Feature Engineering
- Model Evaluation using:
  - MAE
  - R² Score

### Optimization
- Linear Programming with PuLP

---

## Project Structure

```bash
Fantasy-FPL-AI/
│
├── Fantasy_Final.ipynb      # Main notebook containing preprocessing, ML models, and optimization logic
├── sample_output.json       # Example generated team/output
├── screenshots/             # Project screenshots and outputs
├── README.md
└── requirements.txt
```

---

## How It Works

### 1. Data Collection
The project fetches player statistics, fixtures, ownership, and team information using the Fantasy Premier League API.

### 2. Data Preprocessing
The raw data is cleaned and transformed into structured datasets suitable for analysis and prediction.

### 3. Prediction Models
Separate regression-based models are trained using player metrics such as:
- Goals
- Assists
- Expected Goals (xG)
- Clean Sheets
- Saves
- Minutes Played
- Fixture Difficulty

### 4. Squad Recommendation
Using PuLP and linear programming, the assistant generates teams while following official FPL constraints:
- Budget limit
- Formation requirements
- Maximum 3 players per club
- Position limits

---
## 🏆 Example Output

When running the optimizer, the algorithm generates a terminal output detailing the optimal Starting XI, bench configuration, and projected points:

 OPTIMIZED(STARTING 11 + BENCH) 

STARTING XI:
[GK] Raya            | vs CRY (A)   | £ 6.2m | Proj: 5.7
[DEF] Gabriel        | vs CRY (A)   | £ 7.3m | Proj: 5.7
[DEF] Senesi         | vs NFO (A)   | £ 5.2m | Proj: 5.3
[DEF] Guéhi          | vs AVL (H)   | £ 5.1m | Proj: 4.8
[DEF] Truffert       | vs NFO (A)   | £ 4.7m | Proj: 4.6
[MID] Anderson       | vs BOU (H)   | £ 5.6m | Proj: 5.6
[MID] Saka           | vs CRY (A)   | £10.0m | Proj: 5.3
[MID] Enzo           | vs SUN (A)   | £ 6.4m | Proj: 5.1
[MID] Gibbs-White    | vs BOU (H)   | £ 7.5m | Proj: 4.9
[FWD] Haaland        | vs AVL (H)   | £14.7m | Proj: 6.1
[FWD] Watkins        | vs MCI (A)   | £ 8.7m | Proj: 5.1

 BENCH :
 [GK] Dúbravka        | vs WOL (H)   | £ 4.0m | Proj: 2.1
 [DEF] Estève         | vs WOL (H)   | £ 3.8m | Proj: 2.7
 [MID] Anthony        | vs WOL (H)   | £ 5.0m | Proj: 3.4
 [FWD] Kroupi.Jr      | vs NFO (A)   | £ 4.6m | Proj: 4.0
 
 Total Squad Cost:  £98.8m / £100.0m
 STARTING XI Proj Pts: 58.1 pts

## Example Use Cases

- Finding undervalued players
- Planning transfers
- Selecting captains
- Building balanced squads
- Comparing players statistically
- Supporting weekly FPL decisions

---

## Future Improvements

- Advanced ensemble models
- Fixture difficulty weighting
- Transfer recommendation engine
- Captaincy prediction model
- Injury/news integration
- Streamlit or Flask web interface
- Historical season backtesting

---

## Learning Outcomes

Through this project, I gained practical experience in:
- Machine learning workflows
- Data preprocessing
- Regression modeling
- Optimization techniques
- API integration
- Analytics-driven decision systems

---

## Author

**Pranjal Jha**

- LinkedIn: [https://linkedin.com/in/pranjaljha](https://www.linkedin.com/in/pranjal-jha-5a0a052b7/)
- GitHub: https://github.com/G0DLYPJ

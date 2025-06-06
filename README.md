# 🏁 Quali vs Race Performance Analyzer

This quick project compares Formula 1 drivers' qualifying positions to their final race results and calculates a custom **Racecraft Score** — a simple metric to evaluate how much a driver gained or lost during the race relative to their grid position.

---

### 🎯 Objective

To identify which drivers most outperformed (or underperformed) their qualifying positions, using real F1 data.

---

### 📈 Racecraft Score Formula

Racecraft Score = (Quali Position - Race Finish Position) / Quali Position

yaml
Copy
Edit

- A positive score = positions gained
- A negative score = positions lost
- Higher = better racecraft

---

### ✅ What It Does

- Pulls live qualifying and race data using FastF1
- Merges the two datasets by driver
- Computes position change and Racecraft Score
- Visualizes the results in a bar chart
- Exports a CSV file with all the stats

---

### 🧰 Tools & Libraries

- [`fastf1`](https://pypi.org/project/fastf1/)
- `pandas`
- `matplotlib`
- `seaborn`

---

### ⚙️ How to Run

```bash
# 1. Set up virtual environment (optional but recommended)
python3 -m venv .venv
source .venv/bin/activate

# 2. Install dependencies
pip install fastf1 pandas matplotlib seaborn

# 3. Run the script
python main.py
The chart will display automatically, and a CSV file like 2024_Bahrain_racecraft_scores.csv will be saved.

📂 Files
bash
Copy
Edit
main.py                      # Core script
cache/                       # FastF1 cache
2024_Bahrain_racecraft_scores.csv  # Output stats
README.md                    # Project overview
📌 Sample Use Case
An F1 team can use this tool post-race to:

Evaluate drivers’ performance vs. expectation

Identify high racecraft drivers

Analyze qualifying efficiency

🚀 Author
Lance Silliman
Aspiring F1 Team Principal & Strategist
Passionate about race engineering, motorsport data, and developing tools that offer teams a competitive edge.

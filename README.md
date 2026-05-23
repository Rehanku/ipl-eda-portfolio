# IPL Data Analysis & Match Insights (2008-2022)

**Executive Summary:** This project analyzes historical IPL data from 2008 to 2022 to uncover key trends in player performance and match outcomes. The most significant finding reveals that winning the toss has a surprisingly minimal impact on winning the match.

**Data Pipeline:**
- Cleaned and standardized team names across different seasons.
- Handled null values in match outcomes and player details appropriately.
- Merged the delivery-level and match-level datasets for comprehensive analysis.

**Key Insights:**
1. **Top Performers:** A historical breakdown of the most dominant run-scorers and consistent wicket-takers across all 14 seasons.
2. **The "Toss Illusion":** Proving mathematically that winning the pre-match toss only results in winning the match ~51.5% of the time.
3. **The "Chris Gayle Anomaly":** Highlighting the balance between run volume and strike rate, showing Gayle hit 41% more sixes than the #2 player.

**Visualizations:**
[![Insight 1](screenshots/top_wicket_takers.png)](screenshots/top_wicket_takers.png)
[![Insight 2](screenshots/toss_impact.png)](screenshots/toss_impact.png)
[![Insight 3](screenshots/strike_rate_scatter.png)](screenshots/strike_rate_scatter.png)

**How to Run:**
```bash
# Clone the repository
git clone https://github.com/Rehanku/ipl-eda-portfolio.git
cd ipl-eda-portfolio

# Create a virtual environment
python3 -m venv .venv

# Activate the virtual environment
source .venv/bin/activate

# Install the required packages
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook notebooks/01_EDA.ipynb
```

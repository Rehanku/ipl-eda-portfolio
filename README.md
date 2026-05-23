# IPL Data Analysis & Match Insights (2008-2022)

**Executive Summary:** This project analyzes historical IPL data from 2008 to 2022 to uncover key trends in player performance and match outcomes. The most significant finding reveals that winning the toss has a surprisingly minimal impact on winning the match.

**Data Pipeline:**
- Cleaned and standardized team names across different seasons.
- Handled null values in match outcomes and player details appropriately.
- Merged the delivery-level and match-level datasets for comprehensive analysis.

**Key Insights & Strategic Implications:**
1. **Top Performers (Runs & Wickets):** A historical breakdown of the most dominant players across all 14 seasons (e.g., Virat Kohli, Shikhar Dhawan, Lasith Malinga). 
   * **What This Means:** Franchises should prioritize heavy retention budgets for consistent, high-volume accumulators to anchor their teams across multiple seasons.
2. **The "Toss Illusion":** Proving mathematically that winning the pre-match toss only results in winning the match ~51.5% of the time.
   * **What This Means:** This suggests teams should focus their analytical resources on in-match strategy and adaptability rather than relying on pre-match luck.
3. **The "Chris Gayle Anomaly":** Highlighting the balance between run volume and strike rate, showing Gayle hit 41% more sixes than the #2 player.
   * **What This Means:** This demonstrates that raw run totals don't fully capture a player's impact. Strike rate and boundary-hitting ability are equally, if not more, important for T20 success.

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

**🛠️ Skills Demonstrated**
* **Data Wrangling:** Handled missing venue data by dynamically mapping cities to stadiums and optimizing memory by dropping redundant features.
* **Relational Data:** Successfully merged 225,000+ rows of granular ball-by-ball delivery data with match-level outcomes using Pandas.
* **Data Visualization:** Built custom scatter plots and bar charts using Matplotlib and Seaborn to communicate complex anomalies.
* **Business Storytelling:** Translated raw code outputs into actionable, real-world strategic insights for cricket franchises.

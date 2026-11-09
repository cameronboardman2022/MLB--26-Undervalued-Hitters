# MLB 2026 Undervalued Hitters
### Identifying Potentially Overlooked Offensive Value Through Statcast Analytics

**Author:** Cameron Boardman  
**Tools:** Python, pandas, NumPy, Matplotlib, Jupyter Notebook  
**Focus:** Baseball Operations | Player Evaluation | Sports Analytics

## Project Overview

This project examines MLB hitters from the 2024–2026 seasons to identify players whose underlying offensive performance may be stronger than their traditional results suggest.

Using Statcast-derived metrics, including expected weighted on-base average (xwOBA), actual weighted on-base average (wOBA), barrel rate, hard-hit percentage, strikeout rate, and walk rate, the analysis evaluates potential offensive rebound candidates.

The objective is to demonstrate how quantitative analysis can complement traditional scouting and support player evaluation decisions.

## Research Question

Which MLB hitters in 2026 demonstrated underlying offensive indicators that suggest their observed production may not fully reflect their quality of contact?

## Methodology

1. Import and clean MLB hitting datasets for the 2024, 2025, and 2026 seasons.
2. Compare actual wOBA against expected wOBA.
3. Examine barrel rate, hard-hit percentage, and plate-discipline metrics.
4. Evaluate year-over-year trends in contact quality.
5. Apply exploratory scoring criteria to identify potential candidates.
6. Develop individual player profiles and scouting summaries.

The primary expected-performance metric is:

**xwOBA Gap = xwOBA − wOBA**

A positive gap indicates that a player's modeled expected offensive performance exceeded their actual wOBA. It does not guarantee future improvement.

## Final Five Player Evaluations

| Player | 2026 wOBA | 2026 xwOBA | Gap |
|---|---:|---:|---:|
| Brandon Nimmo | .320 | .338 | +.018 |
| Heliot Ramos | .312 | .329 | +.017 |
| Masyn Winn | .283 | .297 | +.014 |
| Shea Langeliers | .347 | .352 | +.005 |
| William Contreras | .330 | .334 | +.004 |

### Key Findings

**Heliot Ramos — Strongest Contact-Quality Improvement**

Ramos increased his barrel rate from 8.8% in 2025 to 13.8% in 2026, while posting a positive .017 xwOBA gap. His improved contact quality provides a meaningful reason for further evaluation.

**Brandon Nimmo — Largest Expected-Performance Gap**

Nimmo recorded a .018 positive xwOBA gap with relatively stable hard-hit and barrel rates. His profile suggests a difference between expected and actual production rather than a substantial improvement in contact quality.

**Masyn Winn — Developmental Evaluation Candidate**

Winn recorded a positive .014 xwOBA gap, but his 3.3% barrel rate indicates limited power-oriented contact quality. His profile warrants additional evaluation rather than a confident rebound projection.

**Shea Langeliers and William Contreras — Established Offensive Contributors**

Both hitters posted positive but relatively small expected-performance gaps. Their inclusion illustrates that the final shortlist contains different types of offensive profiles, not exclusively underperforming hitters.

## Visualizations

The project includes:

- Expected versus actual offensive performance
- Contact-quality comparisons
- Percentile-based player evaluations
- Multi-season offensive trends
- Individual player profile visualizations

## Baseball Operations Applications

This analysis demonstrates a framework that could support:

- Preliminary player acquisition screening
- Identification of potential rebound candidates
- Offensive player-development discussions
- Quantitative scouting reports
- Follow-up video and contextual evaluation

## Limitations

This project is an exploratory analysis rather than a validated predictive model.

Positive xwOBA gaps do not necessarily indicate bad luck or guarantee improved future results. Differences in seasonal samples, playing time, batted-ball characteristics, and other contextual factors can influence the findings.

The scoring criteria are heuristic and have not been independently validated against future performance. Additional research would be needed before using the results for acquisition or roster decisions.

## Repository Contents

- `MLB_Undervalued_Hitters_2026.ipynb` — Main analysis notebook
- `stats.csv`, `stats_2024.csv`, `stats_2025.csv` — Season datasets
- `2026_final_five_player_profiles.csv` — Historical player profiles
- `2026_final_scouting_summary.csv` — Final scouting summary
- `scouting_reports/` — Individual scouting visualizations
- `requirements.txt` — Python dependencies

## Running the Analysis

Install the required packages:

```bash
pip install -r requirements.txt
```

Open `MLB_Undervalued_Hitters_2026.ipynb` in Jupyter Notebook or VS Code and run the analysis cells.

## Author

**Cameron Boardman**

MBA, Business Analytics Concentration — University of Hartford  
BSBA, Sports Management — University of Hartford  
Graduate Certificate in Business Analytics — New Jersey Institute of Technology (in progress)

Division I collegiate baseball player with interests in baseball operations, player development, performance analytics, and data-driven decision-making.

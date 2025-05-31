
# Podcast Listening Behavior Analysis

**Prepared by:** Shahad Bakhsh  
**Dataset Coverage:** 18+ user sessions across podcast episodes, categories, countries, and demographics.

## Overview

This repository contains an in-depth exploratory data analysis (EDA) of podcast listening behavior. The goal is to uncover actionable insights into user engagement, age and gender preferences, repeat behaviors, and regional trends, with the aim of improving content strategy, retention, and platform experience.

## Files

| File Name                            | Description |
|-------------------------------------|-------------|
| `podcast_full_analysis-3.ipynb`     | Full analysis notebook with visualizations and code |
| `Podcast Listening Behavior Key Insights and Actionable Recommendations.pdf` | Executive summary report with insights and recommendations |
| `users.csv`, `episodes.csv`, `listens.json` | Input datasets (assumed for the notebook) |

## Data Preprocessing

- Merged 3 datasets: `users`, `episodes`, `listens`
- Removed duplicates and corrected data types
- Identified and excluded invalid values:
  - 0-second sessions
  - Negative durations or ages
  - Outliers (none found)
- No imputation, scaling, or encoding applied, as the analysis was descriptive.

## Key Analyses

1. Top Categories by Listening Time
   - Sports, Society, and News dominate in listener engagement.

2. Average Listening Duration by Gender
   - Female users listen ~15 min/session vs. ~10.5 for male users.

3. Episodes per User
   - Average: ~4.42 episodes/user; most users consume 4–6.

4. Listening Duration by Age Group
   - Users in their 30s and 40s have the longest and most consistent session times.

5. Gender-Based Category Preferences
   - Shared interest in Society, Sports, and News.
   - Female: Religion & Tech | Male: Politics

6. Repeat Listening Behavior
   - Episode 9: Popular with users in their 20s
   - Episodes 1 & 3: Favored by users in their 40s

7. Listening Time by Country
   - Jordan and Morocco lead in total engagement.

8. Short Sessions (Drop-Off)
   - Common in Egypt, Saudi Arabia, and among male users.

9. Zero-Duration Sessions (UX/Tech Issues)
   - Detected in Jordan and among female users — potential UX issues.

10. Basic Recommendation System
   - Suggests unplayed episodes from top categories. Can be expanded with ML.

## Strategic Recommendations

- Tailor content by age and gender
- Localize content for high-engagement regions
- Optimize intros to reduce early exits
- Conduct UX testing to investigate zero-duration issues
- Promote high-repeat episodes with banners or highlights
- Implement recommendation systems based on user behavior

## Tools & Libraries Used

- Python (Pandas, NumPy)
- Matplotlib, Seaborn
- Jupyter Notebook

## How to Run

1. Clone this repository
2. Ensure you have Python 3 and required libraries installed
3. Launch the notebook:
   ```bash
   jupyter notebook podcast_full_analysis-3.ipynb
   ```

## License

This analysis and report are shared for educational and strategic planning purposes. For commercial usage or further research collaboration, please contact the author.

# fifa-worldcup-analytics-dashboard
Interactive Power BI dashboard analyzing historical FIFA World Cup data, visualizing team performance, goals, win rates, and attendance trends.

⚽ FIFA World Cup Analytics Dashboard

📌 Project Overview

This project presents a comprehensive FIFA World Cup Analytics Dashboard developed using Microsoft Power BI with integrated Python-based advanced analytics.

The dashboard provides insights into team performance, scoring trends, attendance patterns, and advanced statistical analysis using machine learning techniques.

The goal of this project is to combine Business Intelligence + Data Science to perform deep sports analytics.


---

🎯 Objectives

Analyze historical FIFA World Cup match data

Compare home vs away team performance

Evaluate goal-scoring trends across tournaments

Study attendance and possession patterns

Apply statistical analysis and clustering techniques

Build an interactive multi-page Power BI dashboard



---

🛠 Tools & Technologies Used

Microsoft Power BI

DAX (Data Analysis Expressions)

Python

pandas

matplotlib

seaborn

scikit-learn


Excel / CSV Dataset



---

📊 Dashboard Structure (6 Pages)


---

🟢 Page 1: Executive Overview

KPIs Displayed:

Total Goals

Win Rate

Average Attendance

Average Possession


Visuals Used:

KPI Cards

Bar Chart (Goals by Home Team)

Map / Filled Map

Slicers (World Cup Year, Team)


Purpose: Provides high-level tournament summary for quick insights.


---

🟡 Page 2: Goals & Match Trend Analysis

Visuals Used:

Gauge Chart (Win Rate)

Clustered Bar Chart (Home vs Away Goals)

Line Chart (Score Trend)

Waterfall Chart (Goal Difference)


Purpose: Analyzes scoring dominance and match-level trends.


---

🟠 Page 3: Team Performance & Possession Analysis

Visuals Used:

Donut Chart (Goals by Team)

Scatter Plot (Possession vs Goals)

Stacked Column Chart

Area Chart (Goals by Year)


Purpose: Compares team-level attacking and possession performance.


---

🔵 Page 4: Advanced Analytics (Python – Part 1)

Visuals Used:

Correlation Heatmap

Violin Plot

PCA Projection

K-Means Clustering


Purpose: Performs statistical relationship analysis and clustering of match performance metrics.


---

🟣 Page 5: Advanced Analytics (Python – Part 2)

Visuals Used:

3D Scatter Plot

Density Distribution Plot

Rolling Average Trend

Radar Chart (Multi-Metric Comparison)


Purpose: Performs multivariate and trend-based performance analysis.


---

🟤 Page 6: Exploratory & Network Analysis

Visuals Used:

Bubble Matrix Plot

Team Interaction Network Graph

Hexbin Density Plot

Pair Plot


Purpose: Identifies hidden patterns and performance relationships.


---

📂 Dataset Information

Dataset Name: fifa_worldcup_clean_dataset.csv

Key Columns:

match_id

worldcup_year

host_country

home_team

away_team

home_goals

away_goals

goal_difference

possession_home

shots_on_target

total_shots

attendance



---

🧮 Key DAX Measures

Total Goals = SUM(home_goals) + SUM(away_goals)

Total Matches = DISTINCTCOUNT(match_id)

Goal Difference = SUM(home_goals) - SUM(away_goals)

Win Rate =
DIVIDE(
    CALCULATE(COUNTROWS(FIFA), FIFA[goal_difference] > 0),
    [Total Matches]
)

Avg Attendance = AVERAGE(attendance)

Avg Possession = AVERAGE(possession_home)


---

📈 Key Insights Generated

Identification of top goal-scoring teams

Comparison of home vs away scoring efficiency

Strong correlation between shots on target and goals

Clustering of teams based on performance metrics

Trend analysis of scoring behavior across years

Attendance growth pattern analysis



---

🎨 Dashboard Design Features

Clean and consistent color theme

Interactive slicers

Drill-through capability

Cross-filtering between visuals

Combination of BI and Machine Learning visuals

Professional layout and spacing



---

🚀 Project Highlights

✔ Multi-page interactive dashboard
✔ Integration of Power BI with Python
✔ Advanced statistical analysis
✔ Machine learning clustering
✔ Business + Data Science combined
✔ Suitable for Data Analyst / BI Developer portfolio


---

📌 How to Use

1. Open .pbix file in Power BI Desktop


2. Ensure Python scripting is enabled (Options → Python scripting)


3. Refresh dataset


4. Navigate through dashboard pages using page tabs


5. Use slicers to interact with data




---

👨‍💻 Author

Akshay
Aspiring Data Analyst | Power BI Developer | Python Enthusiast



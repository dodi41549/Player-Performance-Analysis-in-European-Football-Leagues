🏆 Player Performance Analysis in European Football Leagues
📌 Project Overview
This project aims to analyze player performance across the top 5 European football leagues (Premier League, La Liga, Serie A, Bundesliga, Ligue 1) using statistical data. It involves preprocessing, exploration, clustering, and visualization of player performance metrics derived from FBref.

The ultimate goal is to uncover player profiles, understand performance patterns by position, and support data-driven talent evaluation strategies using unsupervised learning.

🎯 Objectives
- Clean and structure player performance data from multiple CSV sources.

- Visualize performance distributions by player position.

- Explore correlations between raw attributes and percentile metrics.

- Segment players into meaningful groups using clustering (K-Means).

- Compare top players using Radar (Spider) Charts.

- Prepare the project for public sharing and review via GitHub.

📂 Dataset Details
Source	  : FBreF data from Kaggle ([FBreF data](https://www.kaggle.com/datasets/soulcelestia/fbref-data))
Format	  : CSV (split by player positions)
Scope	    : Unknown Season (probabality on 2022/2023 season)
Positions :	Goalkeepers, Center Backs, Full Backs, Midfielders, Attacking Midfielders / Wingers, Forwards
Attributes:	19 for Non-GK players, 13 for GK players
Extra Info:	Includes percentile values for each attribute

Sample Columns (Attribute Names.txt on folder data) :
For Non-GK     : Non-Penalty Goals, xG, Assists, Shots Total, Progressive Carries, Blocks, etc.

For GK         : PSxG-GA, Save Percentage, Touches, Crosses Stopped %, etc.

🔧 Tools & Technologies
- Python as data manipulation, modeling, & visualization
  - pandas, numpy, matplotlib, seaborn, scikit-learn
- Google Colab as analysis environment
- (Optional) Tableau / Power BI: for interactive dashboards

🧪 Project Pipeline
1. Data Cleaning & Preparation
  - Merged multiple CSV files based on player position.
  - Converted stringified vectors to numerical columns (Attr_0 to Attr_18 for non-GK, Attr_0 to Attr_12 for GK).
  - Added column Position and handled missing values (e.g., using mean imputation).
2. Exploratory Data Analysis (EDA)
  - Visualized attribute distributions by position (e.g., Assists, Progressive Passes).
  - Investigated attribute-to-percentile correlations using heatmaps.
3. Clustering (Player Segmentation)
  - Normalized attribute vectors.
  - Applied K-Means clustering with Elbow Method to determine optimal k.
  - Used PCA to reduce dimensions for visualization.
  - Separated clustering for Non-GK and GK players.
  - Interpreted cluster profiles by attribute mean comparison.
4. Performance Visualization
  - Created Radar (Spider) Charts to compare top players like Messi, Lewandowski, and Ronaldo, etc across multiple attributes.
  - Ranked players by many attribute value such as Non-Penalty Goals and visualized Top 100 scorers using barplots.

📊 Sample Visuals
📈 Bar Chart: Top 100 from many attribute values
🕸️ Radar Charts: Multi-attribute comparison between elite players
🔥 Heatmaps: Attribute-to-percentile correlations
🎯 PCA Scatter Plots: Player clusters

📈 Future Work
- Integrate market value data to identify undervalued/overvalued players.
- Build interactive dashboards for scouting use.
- Extend clustering by combining positional + performance + age data.

👤 Author
Analyst: ([@Dodi Al farisy](https://github.com/dodi41549))
Date: Mei 2025

📎 License
This project is open-source and available for educational and professional portfolio use.


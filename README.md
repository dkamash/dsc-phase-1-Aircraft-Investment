________________________________________
Aviation Accident Risk Analysis
This project analyzes aviation accident data to identify patterns and compute risk indices for different aircraft makes and models. The goal is to provide a data-driven evaluation of aircraft safety profiles.
________________________________________
Overview
The dataset contains historical aviation accident and incident records. We focus on:
•	Cleaning and filtering accident-related records
•	Computing risk factors for each aircraft make/model
•	Visualizing accident severity trends and safety profiles
________________________________________
Key Objectives
1.	Load and explore the aviation accident dataset.
2.	Clean and prepare the data for analysis.
3.	Calculate key safety metrics:
o	Fatality Index
o	Injury Index
o	Damage Severity Index
4.	Compute a Risk Score based on weighted indices.
5.	Visualize trends, distributions, and top-performing aircraft.
________________________________________
Tech Stack
•	Programming Language: Python 3
•	Libraries:
pandas, seaborn, matplotlib
________________________________________
Dataset
•	Source: data/Aviation_Data.csv
•	Content: Aircraft type, accident details, injuries, damage status, and related metadata.
________________________________________
Data Preparation
•	Filtered dataset for Accidents only.
•	Removed records missing critical fields: Make, Model, Aircraft.Category, injury counts.
•	Converted numeric columns and handled missing values.
•	Grouped data by Make and Model to summarize accident and injury statistics.
________________________________________
Risk Model
The following metrics were calculated:
•	Fatality Index:
fatalities / total people onboard
•	Injury Index:
(serious + minor injuries) / total people onboard
•	Damage Severity Index:
destroyed aircraft / total accidents
Weighted Risk Score:
risk_score = (fatality_index * 0.5) +
             (damage_severity_index * 0.3) +
             (injury_index * 0.2)
________________________________________
Visualizations
•	Correlation heatmap of risk factors
•	Indice risk correlation
•	Top 10 lowest-risk aircraft models
________________________________________
How to Run
1.	Clone the repository:  https://github.com/dkamash/dsc-phase-1-Aircraft-Investment.git 
2.	Install dependencies:
pip install -r requirements.txt
3.	Run the notebook or Python script to reproduce analysis.
________________________________________
Sample Output
•	Correlation Heatmap
•	Indice risk correlation
•	Top 10 Aircraft Models (Bar Chart)
________________________________________
License
This project is open-source.
________________________________________


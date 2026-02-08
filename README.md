NBA Team Wins Regression Analysis
Project Overview

This project analyzes which team performance metrics best explain total wins in the NBA. The goal of the analysis is to evaluate how strongly team skill rating, scoring output, and performance differentials relate to season success.

Using historical NBA team data, this project applies correlation analysis and linear regression modeling to determine which variables are most predictive of team wins.

The central question explored in this project is:

What metrics best explain why some NBA teams win more games than others?



Dataset:

The dataset contains historical NBA team statistics including:

-Average points scored per game (avg_pts)
-Average opponent points allowed (avg_opp_pts)
-Average Elo rating representing relative team skill (avg_elo_n)
-Average opponent Elo rating (avg_opp_elo_n)
-Average point differential (avg_pts_differential)
-Average Elo differential (avg_elo_differential)
-Total season wins (total_wins)
-The dataset includes 618 observations across multiple NBA seasons.

Dataset location: data/nba_wins_data.csv



Methods Used

The analysis includes:

-Exploratory data analysis using scatter plots
-Pearson correlation analysis
-Simple linear regression
-Multiple linear regression
-Model comparison using R squared values

Python libraries used:

-NumPy
-Pandas
-SciPy
-Matplotlib
-Statsmodels



Key Visualizations:


-Total Wins vs Average Relative Skill (Elo Rating)

This visualization shows a strong positive relationship between team Elo rating and total wins.
The Pearson correlation coefficient is approximately 0.91, indicating that relative team skill is a strong predictor of season success.


-Total Wins vs Average Points Scored

Average points scored shows a moderate positive relationship with total wins, with a correlation of approximately 0.48.
This suggests scoring alone does not explain team success as strongly as overall team strength.



Regression Results:

A simple linear regression using Elo rating alone produced an R squared value of approximately 0.82, meaning Elo rating explains a large portion of the variation in total wins.
Multiple regression models including scoring and performance differentials improved model performance. The final model achieved an R squared value of approximately 0.88, indicating that performance differentials provide additional explanatory power beyond scoring averages alone.









Project Structure:

nba-team-wins-regression/

data/
nba_wins_data.csv

images/
elo_vs_wins.png
points_vs_wins.png

notebooks/ nba_team_wins_regression.ipynb

reports/ nba_team_wins_report.html

.gitignore







How to Run the Project
Option 1: View Results (Recommended)

Open the HTML report directly in a browser: reports/nba_team_wins_report.html


Option 2: Run the Notebook

Clone the repository: git clone https://github.com/justin-m-richardson/nba-team-wins-regression.git

Navigate into the project folder: cd nba-team-wins-regression

Install required packages: pip install numpy pandas scipy matplotlib statsmodels jupyter

Launch Jupyter Notebook

Open: notebooks/nba_team_wins_regression.ipynb

and run all cells. 



Author

Justin Richardson
Computer Science Student, Southern New Hampshire University

Interests include data analytics, software development, and applied statistical modeling.

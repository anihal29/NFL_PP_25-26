# NFL Playoff Prediction Model

Machine learning pipeline to predict NFL playoff game outcomes for the 2025-26 Season using regular-season play-by-play data.

## Author
Ayaan Nihal

## Goal
Use 2025 NFL regular-season play-by-play data to build a team-level prediction model for postseason matchups. Evalutation done 
with number of games predicted correctly.

## Steps
- Loaded and cleaned 2025 NFL play-by-play data
- Filtered regular-season games for training data
- Aggregated play-level data into team-level offensive, defensive, and special teams statistics
- Engineered matchup-based feature differentials by subtracting away-team statistics from home-team statistics
- Trained a Logistic Regression model to predict whether the home/higher-seeded team would win
- Generated win probabilities for each playoff matchup

## Features Engineered
Key features included:
- Win rate
- Plays per game
- Points per drive
- Points allowed per drive
- Yards per play
- Yards allowed per play
- Third-down conversion rate
- Third-down conversion rate allowed
- Sack rate allowed
- Sack rate forced
- Red-zone touchdown rate
- Red-zone touchdown rate allowed
- Turnovers committed per drive
- Turnovers forced per drive
- Explosive play rate
- Explosive play rate allowed
- Negative play rate
- Starting field position
- Field goal percentage
- Punts per drive

## Model
The final model used Logistic Regression to estimate win probabilities for postseason games based on team-stat differentials.

## Results
11/13 Postseason Games correctly predicted:
-  4/6 Wild Card accuracy
-  4/4 Divisional accuracy
- 2/2 Conference Championship accuracy
- Correctly identified the Super Bowl winner

## Data Sources
Dataset derived from <a href = "https://github.com/nflverse/nflverse-data/releases/download/pbp/play_by_play_2025.csv.gz"/>nflverse</a>

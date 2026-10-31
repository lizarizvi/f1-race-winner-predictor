# F1 Race Winner Predictor

My first machine learning project. It predicts who will win the next Formula 1 Grand Prix, using race results from 2021 to 2026 (downloaded from the free Jolpica-F1 API).

### How it works

**Features:** grid position, plus each driver’s average finish, wins and points over their previous 5 races, and the team’s recent points.

**Model:** Random Forest, with encoding for drivers, teams and circuits.

**Test:** trained on earlier races and tested on the last 6 of 2026, so the model never sees the future.

**Limits:** Six test races is a tiny sample, so the score is a rough guide. The model has no qualifying lap-time gap, practice pace, weather or strategy data.

### Predictions

mexico_pre_quali: before qualifying, so grid position is missing.
mexico_post_quali: added after qualifying.
Next: qualifying gap, practice long-run pace, walk-forward validation, XGBoost.

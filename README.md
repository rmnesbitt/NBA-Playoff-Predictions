# NBA Stats Analysis

Predicting Playoff Participation and Championship Wins from Regular Season Statistics

---

## Purpose

This project explores whether a team's regular season performance metrics can predict their likelihood of making the playoffs or winning the NBA championship. Two machine learning models were trained using historical game data to evaluate how well statistical indicators translate into postseason success.

---

## Tools & Techniques

**Languages & Libraries:**  
Python, SQLite, pandas, matplotlib, seaborn, scikit-learn, imbalanced-learn (SMOTE)

**Techniques Used:**
- Data extraction from relational database (SQLite)
- Feature engineering from game-level stats
- Principal Component Analysis (PCA) for visualization
- SMOTE for addressing class imbalance
- Logistic Regression for playoff prediction
- Random Forest for championship prediction
- Evaluation via accuracy, precision, recall, and F1-score

---

## Key Insights

- The **playoff participation model** achieved an accuracy of 68.25%.  
- The **championship prediction model** achieved a high overall accuracy of 98.33%, but this was heavily skewed due to class imbalance (only a few teams win championships).
- Feature engineering on stats such as field goal %, 3-point %, free throw %, and points scored provided predictive signal.
- PCA visualization clearly clustered teams based on regular season performance, with playoff teams and champions forming distinct groups.
- The models suggest that playoff participation is easier to predict than championship wins, which are more variable.

---

## Sample Prediction

Given a new team’s regular season statistics, the models can estimate:

- **Playoff Probability:** 99.99%  
- **Championship Win Probability:** 41.00%

These values offer interpretable outputs for analysts, coaches, or fans.

---

## Project Structure

- **Data Extraction & Preparation:** Loads historical NBA data and computes team-level aggregates.
- **Visualization Script:** Performs PCA and annotates team clusters by playoff/championship status.
- **Model Training & Prediction:** Builds and evaluates machine learning models for classification tasks.

---

## Personal Takeaways

- Learned to balance imbalanced classification using SMOTE  
- Improved PCA interpretation and clustering visualization techniques  
- Gained experience connecting SQL-based data sources to predictive pipelines  
- Practiced building interpretable sports analytics models that highlight data limitations

---

## Contact

Ryan Nesbitt  
rmnesbitt@gmail.com  
https://www.linkedin.com/in/rmnesbitt  
http://rmnesbitt.github.io

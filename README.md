# OKC Thunder Win/Loss Prediction Using Machine Learning

## Project Overview

This project explores whether machine learning models can predict whether the Oklahoma City Thunder will win or lose a game based on historical team statistics. The goal is not to create a perfect predictor, but to understand how structured basketball data can be used for classification and how different machine learning models behave on the same problem.

Rather than focusing on player-level narratives or betting applications, this project treats the problem as a learning exercise in applied machine learning: data preparation, feature selection, model training, evaluation, and interpretation.

---

## Project Goals

- Build a complete, end-to-end machine learning workflow
- Practice cleaning and preparing real-world sports data
- Compare multiple classification models taught in class
- Evaluate models using accuracy and confusion matrices
- Understand the trade-offs between simple and complex models

---

## Dataset Description

The dataset consists of historical NBA **team-level game statistics**, where each row represents a single team’s performance in a single game. The target variable is whether the team **won or lost** that game.

Only team-level data is used in this project. While player-level statistics are available, they were intentionally excluded to keep the scope focused and aligned with course material.

Key characteristics of the dataset:
- One row per team per game
- Numerical features describing team performance
- Binary outcome variable (Win / Loss)
- Filtered to recent seasons to better reflect modern team composition

---

## Data Preparation and Cleaning

Before modeling, the dataset was carefully prepared to ensure consistency and relevance:

- Filtered the data to focus on recent seasons
- Selected team statistics that logically relate to game outcomes
- Converted categorical outcomes into binary labels
- Checked for missing values and data integrity issues
- Ensured features were suitable for classification models

The intent during preprocessing was not to over-engineer the data, but to create a clean and interpretable feature set that reflects how teams perform on the court.

---

## Models Used

The following machine learning models were implemented and compared:

- **Logistic Regression**  
  Used as a baseline model due to its simplicity and interpretability.

- **Decision Tree Classifier**  
  Used to capture non-linear relationships between features.

- **Naive Bayes**  
  Used as a probabilistic baseline model.

- **Neural Network (MLP)**  
  Used to explore whether a more flexible model could capture additional patterns.

Each model was trained and evaluated using the same dataset split to allow fair comparison.

---

## Model Evaluation

Model performance was evaluated using:

- **Accuracy** – to measure overall correctness
- **Confusion Matrix** – to understand the types of errors made

Using multiple evaluation tools helps avoid misleading conclusions that can arise from relying on accuracy alone, especially in classification problems where different types of errors matter.

---

## Key Findings

- Simpler models, particularly Logistic Regression, performed competitively compared to more complex models.
- Increased model complexity did not always lead to better performance.
- Team-level statistics contain meaningful signals, but also clear limitations.
- The results highlight the importance of feature quality over model complexity.

---

## Limitations

This project has several important limitations:

- Player injuries, roster changes, and coaching decisions are not included.
- Team statistics may not fully capture game context or momentum.
- The model is not intended for real-world betting or forecasting use.
- Results are dependent on the selected seasons and features.

These limitations are expected and reinforce the exploratory nature of the project.

---

## Future Improvements

Possible directions for future work include:

- Incorporating player-level statistics
- Adding opponent-specific matchup features
- Using time-aware validation instead of random splits
- Exploring additional feature engineering techniques

---

## Author

**Isaac Wanlemvo**  
Software Engineering & AI Student  
Focus: Applied Machine Learning, Data Systems, and Real-World Modeling

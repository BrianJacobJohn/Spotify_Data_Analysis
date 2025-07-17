# Spotify Danceability Analysis 🎶

**Can we predict how danceable a song is based on its acoustic features?**

This project uses Spotify’s open dataset (via TidyTuesday) and explores which features most strongly influence a song's "danceability" score. Using linear regression, LASSO, and interaction models, we evaluate statistical relationships and assess how well we can model subjective musical experiences.

---

## 🔍 Objective
> To identify the key acoustic and structural characteristics of songs that contribute to their danceability score using statistical modeling techniques.

---

## 📊 Techniques Used
- Multiple Linear Regression (base model)
- LASSO Regularization
- Interaction Term Modeling
- Diagnostic Plots & Assumption Checks
- Model Improvement via R², GVIF, and ANOVA

---

## 📁 Dataset
- 32,833 songs from Spotify's internal metrics via [TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-01-21/readme.md)
- 23 features including loudness, energy, valence, tempo, key, speechiness, and more.

---

## 💡 Key Insights
- **Valence**, **speechiness**, and **tempo** had the strongest positive relationships with danceability.
- The base model had an **adjusted R² of 0.248**, which increased to **0.35** with first-order interactions.
- Residual analysis revealed violations in **independence** and **normality**, and presence of **influential points**.
- Despite statistical significance of predictors, the model struggled with explanatory power, suggesting deeper cultural or psychological factors at play.

---

## 📈 Future Work
- Use non-parametric models (e.g., random forest, XGBoost)
- Expand to **multi-year Spotify Wrapped data** for time series modeling
- Add a **Streamlit app** for interactive danceability exploration

---

## 📎 Files
- `Spotify_Danceability_Analysis.qmd`: Contains full analysis, model building, diagnostics
- `figure-markdown_github/`: Visual outputs used in this README
- `data/`: Source and processed datasets

---

## Note

I and my collaborator Like built this project not just to satisfy assignment requirements, but to explore the line between numbers and nuance — what can data tell us about human movement, taste, and emotion? This is part of my broader effort to make storytelling through data more accessible and human.

For feedback or collaboration ideas, feel free to reach out!

# Video Game Hit Analysis & Prediction

## Overview

This project analyzes historical video game sales data to identify patterns associated with commercial success. A game is classified as a **hit** if its global sales reach at least 1 million units.

The analysis examines how hit rates vary across game genres and platforms and evaluates whether critic scores can help predict a game's likelihood of becoming a hit.

## Research Questions

- Which genres and platforms have the highest hit rates?
- Is critic score associated with the probability of a game becoming a hit?
- Can logistic regression provide an interpretable prediction of hit probability?

## Dataset

The dataset contains **17,495 video game releases from 1980 to 2024**.

Key variables include:

- `Genre`
- `Platform`
- `Global_Sales`
- `Critic_Score`
- `Year_of_Release`

A binary target variable, `Hit`, was created:

- `Hit = 1`: Global sales ≥ 1 million units
- `Hit = 0`: Global sales < 1 million units

Only approximately **8.6% of games** in the dataset were classified as hits.

## Methods

- Data cleaning and missing-value assessment
- Exploratory data analysis
- Hit-rate comparison by genre and platform
- Logistic regression for hit prediction
- Confidence interval estimation
- Data visualization using `ggplot2`

## Key Findings

- Shooter games had the highest hit rate among the major genre groups, at approximately **18%**.
- Action-Adventure games also showed a relatively high hit rate, at approximately **14%**.
- Critic score was strongly associated with hit probability.
- Each one-point increase in critic score was associated with approximately **2.5 times higher odds** of becoming a hit, with a 95% confidence interval of approximately **2.3 to 2.7**.

These findings describe associations in the dataset and should not be interpreted as proof that critic scores directly cause higher sales.

## Visualizations

The project includes visualizations of:

- Hit rate by genre
- Hit rate by platform
- Predicted hit probability by critic score
- Distribution of global sales
- Relationship between critic score and hit status

## Tools

- R
- `tidyverse`
- `dplyr`
- `ggplot2`
- Logistic regression

## Limitations

- The dataset is observational, so causal conclusions cannot be established.
- Many games have missing critic scores or release years.
- Sales may be influenced by marketing budget, publisher reputation, franchise popularity, release timing, and platform reach.
- The definition of a hit depends on the selected 1-million-unit threshold.
- Historical sales patterns may not fully represent the current video game market.

## Project Structure

```text
video-game-hit-analysis/
├── data/
├── scripts/
├── figures/
├── report/
├── README.md
└── video_game_hit_analysis.Rmd
```

## Author

My Cao  
M.S. Statistical Data Science, San Francisco State University

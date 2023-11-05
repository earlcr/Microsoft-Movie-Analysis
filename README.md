![Alt Microsoft Logo](https://github.com/earlcr/Microsoft-Movie-Analysis/blob/template-mvp/images/microsoft%20logo.jpg)
# Microsoft Movie Investment Analysis

**Author**: Earl Chirchir

## Overview

This project conducts an in-depth analysis of historical box office data to uncover patterns linking movie genres, ratings, votes, and revenues. The goal is providing Microsoft actionable insights as it enters the movie industry, guiding data-driven investments for maximizing financial returns. The analysis utilizes descriptive statistics and visualizations to reveal genres, franchises, and quality ratings strongly correlate with box office success.

## Business Problem

As Microsoft launches its new movie studio, the business needs to make smart investments in film projects that will resonate with audiences and generate strong box office revenues. However, as a new entrant to the movie industry, Microsoft currently lacks insights into what specific movie attributes and strategies correlate with financial success.

This analysis aims to uncover patterns in historical movie data that can inform Microsoft's investment decisions when selecting movie ideas, setting budgets, and allocating marketing resources. Focusing on proven formulas and genres for success can help mitigate the inherent risk in film production and marketing.

Specific business questions this analysis aims to answer:

-  What film genres, based on historical data, have consistently delivered the highest box office revenues? This will help guide genre selection.
-  Do sequels and franchise films reliably outperform non-sequel movies in terms of gross sales? This will inform franchise strategy.
-  How do factors like ratings and number of user votes correlate with overall box office performance? This will shape marketing tactics.
-  What production budgets and marketing spends have been associated with highly profitable movies? This will set spending guardrails.

These questions are critical for Microsoft Studios to ensure its multimillion dollar movie investments are allocated to projects with the highest revenue potential. By leveraging data-driven insights into the key drivers of box office success, Microsoft can refine its strategy across content selection, franchises, marketing, and budgets.

The goal is leveraging patterns linking genres to revenues to optimize Microsoft's genre selection strategy. This will maximize return on investment as the studio enters the industry.

## Data

The analysis uses three datasets:

-  **bom.movie_gross.csv** - Contains box office revenue data for over 7,000 movies. Key variables are 'title', 'studio', 'domestic_gross', and 'foreign_gross'.
-  **title.basics.csv** - Provides movie metadata like 'original_title', 'runtime_minutes', and 'genres' for over half a million titles.
-  **title.ratings.csv** - Includes audience ratings data with variables like 'averagerating' and 'numvotes'.

The target variable is the total box office gross revenue, calculated by summing 'domestic_gross' and 'foreign_gross'.

Key preparation steps included:

-  Dropping rows in gross dataset missing the studio name to enable analysis by studio.
-  Imputing numeric columns like domestic gross with median values to fill in gaps.
-  Ensuring data types were appropriate, converting foreign gross to numeric after removing commas.
-  Merging all datasets using title and tconst as common unique keys.
-  Adding a calculated total gross column by summing domestic and foreign gross.
-  Creating a franchise flag column in merged dataset to enable franchise analysis.

These choices focused on complete cases, maintained data integrity, enabled merging, and engineered features for additional insights.

## Methods

The analysis methodology focused on:

-  Leveraging descriptive statistics including mean, median, and standard deviation to summarize revenues across genres.
-  Employing visualizations such as bar charts, scatterplots, and histograms to uncover patterns and relationships in the data.
-  Calculating averages, percentages, and thresholds for key metrics like user ratings.
-  Using groupby operations and merging to connect data across datasets and analyze different cuts.

Key analysis plots included:

-  Bar chart showing average gross revenue for top genres.
-  Grouped bar chart of franchise vs non-franchise average gross revenue.
-  Scatterplot relating ratings, votes, and high gross revenue movies.

This approach extracted insights from the data without requiring predictive modeling or machine learning.

## Results

Key results and insights from the analysis included:

-  Movies in the Adventure, Animation, and Action genres had the highest average gross revenues, with each exceeding $950 million.
-  On average, movies in a franchise earned over $800 million more than non-franchise films.
-  Movies with user ratings exceeding 7.5 and votes over 100,000 associated strongly with high box office gross revenue above $500 million.
-  The Sweetspot for high box office success was ratings between 7.5-8.5 and votes greater than 250,000.

These insights provide Microsoft with a data-backed investment thesis for maximizing returns. Limitations include incomplete revenue data and rapidly changing industry conditions affecting generalizability.



## Conclusions

Based on the analysis, the recommendations for Microsoft's movie investments are:

-  Focus on proven high-revenue genres like Adventure, Animation, and Action for core studio projects.
-  Develop franchises with sequels and leverage existing intellectual property to build fan affinity.
-  Prioritize releasing quality films with strong engagement to drive audience ratings and reviews.

Implementing these data-driven recommendations can significantly increase Microsoft's probability of box office success for its upcoming slate of original movies.

The analysis provides a template for continually leveraging data to guide Microsoft's movie investments as the studio matures. But constant vigilance is required given the dynamic nature of the entertainment industry.




## Repository Structure

Description of the structure of the repository and its contents:

```
├── README.md                                   <- The top-level README for reviewers of this project
├── microsoft_movie_investment_analysis.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── microsoft_movie_investment_presentation.pdf <- PDF version of project presentation
├── zippedData                                  <- Both sourced externally and generated from code
└── images                                      <- Both sourced externally and generated from code
```

# Microsoft Movie Investment Analysis

**Author**: Earl Chirchir

## Overview

This project conducts an in-depth analysis of historical box office data to uncover patterns linking movie genres, ratings, votes, and revenues. The goal is providing Microsoft actionable insights as it enters the movie industry, guiding data-driven investments for maximizing financial returns. The analysis utilizes descriptive statistics and visualizations to reveal adventure, animation, action, franchises, and quality ratings strongly correlate with box office success.

## Business Problem

As Microsoft launches its movie studio, data-driven analytics are required to inform multimillion-dollar investment decisions across projects and genres. Specifically, the analysis aims to answer:

-  Which specific genres have consistently generated the highest average domestic and international gross revenues?
-  How do user ratings on sites like IMDb correlate with overall financial performance for different movie genres?
-  How many user votes on rating sites associate with box office success for different genres?
-  Can these detailed genre insights guide Microsoft's project selection for the highest probability of box office success?

The goal is leveraging patterns linking genres to revenues to optimize Microsoft's genre selection strategy. This will maximize return on investment as the studio enters the industry.

## Data

The data includes three key datasets:

-  Movie box office gross revenue data for over 7,000 films, including variables like title, studio, domestic gross, and foreign gross.
-  Movie metadata for over half a million titles, including original title, runtime, and genres.
-  Movie ratings data with variables like average rating and number of votes.

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
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```

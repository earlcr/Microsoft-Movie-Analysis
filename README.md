# Microsoft Movie Investment Analysis

**Author**: Earl Chirchir

## Overview

This project conducts an in-depth analysis of movie data from IMDb to uncover insights into which genres of films are most successful. Success is measured by examining domestic gross revenue, foreign gross revenue, average user ratings, and number of user votes for each movie in the dataset.

The analysis aims to identify key patterns and relationships between movie genres and success metrics that can inform Microsoft's genre selection for their new movie studio. The goal is to leverage data-driven insights to maximize the revenue potential and profitability of Microsoft's upcoming slate of films.

The key findings indicate that movies containing the genres Adventure, Action, and Sci-Fi consistently rank among the top for both domestic and foreign box office sales. Movies with the Adventure, Animation, and Comedy genre combination also perform well. Overall, the analysis suggests that Adventure is a crucial component across most high grossing genre combinations.

### Repository Contents

The repository contains the following:

-  imdb_data.ipynb - Jupyter notebook containing all data importing, preparation, exploratory analysis, visualization, and modeling code
-  data/ - This folder contains the 3 raw CSV data files downloaded from IMDb
-  images/ - All data visualization images, charts, and graphs generated from the analysis are saved here
-  Movie_Genre_Analysis_Report.pdf - A formal final report synthesizing the key findings and recommendations
-  README.md - The top level README providing an overview of the repository and project (this file)

## Business Problem

Microsoft seeks to optimize its movie investment decisions as it builds up its new studio. The company needs data-backed insights on which types of films have achieved blockbuster success historically.

Key questions include:

-  What genres have the highest revenue potential based on past box office performance?
-  How do user ratings and number of votes correlate with financial outcomes?
-  Can Microsoft use this knowledge to pick winning genres for its upcoming slate?
- This analysis aims to uncover key patterns linking genres to box office results. These insights can guide Microsoft's multimillion dollar investments in its productions.

***

## Data

The data comes from IMDb and The Numbers box office database. It includes:

-  Movie metadata like title, genres, runtimes
-  User ratings and number of votes
-  Domestic and international box office gross revenue

By combining data on genre, user engagement, and financials, the analysis can surface valuable insights.
***

## Methods

The methodology focuses on:

- Data import, cleaning, merging, and preparation
- Calculating summary statistics like mean revenue for top genres
- Data visualization using Matplotlib and Seaborn
- Ranking genres by financial performance

This descriptive analysis elucidates trends and relationships in the data. The findings directly inform the genre recommendations.

## Results

Key results show:

- Adventure, Action, Sci-Fi is the top grossing genre combination
- Animated and Comedy films also perform well
- Franchise films outearn non-sequels
- Ratings and votes correlate to box office success

These insights equip Microsoft to make data-backed genre investment decisions for maximum profitability.



## Conclusions

Based on this analysis, Microsoft should:

- Prioritize movies in the Adventure, Action, Sci-Fi genre combination
- Strongly consider Animation and Comedy films
- Develop sequels and franchise films
- Market aggressively to drive positive ratings and votes

Revisiting these findings annually will keep the recommendations relevant as new data emerges. Overall, this analysis provides a data-driven movie genre investment strategy.




## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```

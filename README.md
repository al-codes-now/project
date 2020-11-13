

# Microsoft Film Studio Business Recommendations

**Authors:** Alexandra Bruno & Davida Rosenstrauch

## Overview

This project analyzes data from films released in the past 20 years in order to inform recommendations for Microsoft's new movie studio. Exploratory analysis shows that films with certain genres and run times are more likely to have desirable revenue, budgets, and imdb ratings.  We recommend Microsoft use these results to inform their production decisions within their new studio.

### Business Problem

We seek to answer the following questions to provide recommendations to Microsoft regarding which types of films  to produce in their new studio:
1. What effect does movie runtime have on revenue, budget, and ratings?
2. What effect does movie genre have on revenue, budget, and ratings?

### The Data

The data used for this analysis were obtained from The Movie Database and The Open Movie Database. Both databases are community built, the data maintence and contribution comes the users of these websites. These data provided us valuable information about tens of thousands of films over the past century. The primary data we used was film revenue, budget, imdb ratings, runtime, and genres.

### Methods

This project uses exploratory data analysis to examine potential factors that can contribute to the sucess of Microsoft's new movie studio. We analyzed two variables, runtime and genre against revenue, budget, and Imdb ratings to determine which runtimes and genres would be most desirable in the films Microsoft chooses to produce.

It should be noted while considering results based on Imdb ratings that there is a very large standard deviation in vote counts for these ratings. "Vote counts" refers to the number of individuals who rated a film on Imdb, whic ultimately contribute to the mean ratings in our data. Given this large standard deviation of 118,421, some ratings will be more indicative than others.

**histogram image**

### Results 

Longer runtimes do not guarantee higher revenues. Additionally, they are less likely to be cost effective.

![runtime_rev](./picsforrm/runtime_rev.png)
![runtime_rev](https://github.com/al-codes-now/project/blob/master/picsforrm/runtime_rev.png)

img src="runtime_rev.png"

img src="Runtime_Budget.png"

On average, the longer a movie’s runtime is the higher the movie’s budget and revenue will be

img src="avg.png"

There is a positive relationship between runtime and ratings 

To encourage higher ratings, the data suggests that longer movie runtimes can be beneficial 

img src="runtime_rating.png"

Highest-rated genre:  Documentary.
Lowest-rated genre: Horror.

img src="mean_ratings_genre.png"

Though higher revenues are correlated with higher budgets, revenues vary more by genre than budgets do. Net profit is 
therefore likely to increase with increased budget.

img src="rev_budg_genre.png"


### Conculsion 

We recommend producing films with runtimes between 100 and 150 minutes in order to optimize likelihood of high revenue and ratings.
We recommend producing films primarily in the genres of Adventure, Fantasy, Science, Fiction, and Family, or a combination of several, in order to optimize likelihood of high revenue.
Though documentaries have shown nearly the lowest revenue numbers as compared to other genres, they also have shown the highest ratings. We therefore recommend producing at least some documentaries for the sake of reputation and name recognition.


### Next steps 

With more time, we would be interested to explore:
1. Controlling for vote counts
2. How any of these trends have changed over time
3. Runtimes’ and genres’ impact on net profits
4. Release dates' impact on revenue, budget, ratings, and net profits
5. Explore correlation between financial success (revenue and/or net profits) and ratings

### Repository Structure

├── picsforrm
├── README.md
├── Microsoft_Notebook.ipynb
├── Microsoft_Presentation.pdf
├── budget_since2010.csv
├── full_df.csv
├── rating_since2010.csv
└── revenue_since2010.csv

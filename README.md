

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

This project uses exploratory data analysis to examine potential factors that can contribute to the sucess of Microsoft's new movie studio. We analyzed two variables, runtime and genre, against revenue, budget, and Imdb ratings to determine which runtimes and genres would be most desirable in the films Microsoft chooses to produce.

It should be noted while considering results based on Imdb ratings that there is a very large standard deviation in vote counts for these ratings. "Vote counts" refers to the number of individuals who rated a film on Imdb, whic ultimately contribute to the mean ratings in our data. Given this large standard deviation of 118,421, some ratings will be more indicative than others.

![histogram](./picsforrm/histogram.png)

### Results 

#### Revenue, Budget, and Ratings by Runtimes 
As shown below, longer runtimes do not guarantee higher revenues, though films are most likely to have high revenue with runtimes between 100 and 150 minutes. Additionally, they are less likely to be cost effective with runtimes longer than this given the stronger correlation between budget and runtimes than between revenue and runtimes, as shown by a steeper regression line in the second figure below.

![runtime_rev](./picsforrm/runtime_rev.png)

![Runtime_Budget](./picsforrm/Runtime_Budget.png)

As shown below, on average, the longer a movie’s runtime is the higher the movie’s budget and revenue will both be. The unusually high "180-210 mins" bar below can be explained by the one outlier shown above, which has a large impact given the few films with very large runtimes. Without this outlier, this final bar would be lower than its immediate predecessors. 

![avg](./picsforrm/avg.png)

As shown below, there is a positive relationship between runtime and ratings 

To encourage higher ratings, the data suggests that longer movie runtimes can be beneficial.

![runtime_rating](./picsforrm/runtime_rating.png)

#### Revenue, Budget, and Ratings by Genre

We see below that Documentaries are the highest-rated genre. These could therefore be beneficial movies to produce to gain popularity and and a positive reputation as a studio.

![mean_ratinngs_genre](./picsforrm/mean_ratings_genre.png)

As seen below, though higher revenues are correlated with higher budgets, revenues vary more by genre than budgets do. Net profit is therefore likely to increase with increased budget. Adventure movies show the highest revenue, and interestingly, Documentaries bring in more revenue only than one other genre, TV Movies, despite their positive ratings noted above.

![rev_budg_genre](./picsforrm/rev_budg_genre.png)



### Conculsion 

Based on the above data, we offer the below concrete recommendations:

1. We recommend producing films with runtimes between 100 and 150 minutes in order to optimize likelihood of high revenue and ratings.
2. We recommend producing films primarily in the genres of Adventure, Fantasy, Science, Fiction, and Family, or a combination of several, in order to optimize likelihood of high revenue.
3. Though documentaries have shown nearly the lowest revenue numbers as compared to other genres, they also have shown the highest ratings. We therefore recommend producing at least some documentaries for the sake of reputation and name recognition.


### Next steps 

With more time, we would be interested in exploring:
1. Controlling for vote counts
2. How any of these trends have changed over time
3. Runtimes’ and genres’ impact on net profits
4. Release dates' impact on revenue, budget, ratings, and net profits
5. Explore correlation between financial success (revenue and/or net profits) and ratings

### Repository Structure

── picsforrm
── Microsoft_Notebook.ipynb
── Microsoft_Presentation.pdf
── README.md
── budget_since2010.csv
── full_df.csv
── rating_since2010.csv
── revenue_since2010.csv

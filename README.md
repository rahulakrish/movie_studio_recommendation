# Movie Studio startup
This notebook sets out to demonstrate some of the typical data wrangling steps one might undertake in a data science project as well some Pandas and Matplotlib functionality.
By taking up a business case of recommending movies to produce to a new studio, we will see how a dataset processed before conducting an analysis. We will also how web scraping can be useful in the absence of
good quality data.
  
## Data Source
Data was sourced from [Opus Data](https://www.opusdata.com/), the gorup responsible for [The Numbers](https://www.the-numbers.com/). While most of their data is proprietary, they do provide an 'extract' that we can make use of. The file is titled *'MovieData.csv'*.
 
## Defining success
To keep things simple, the analysis is focused solely on revenue generated and thereby maximum profitability.

## EDA
Following were the conculsions form the intial EDA:

1. Data spanned the years 2006-2018:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/0a259f4b-173a-45ae-bbd2-93bf89adb013)

2. Drama was the most popular genre that was produced:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/9917e7df-0fcd-4108-a215-4c577052e5b7)

3. Median budget was approx. $50 million. Outlier was movie(s) with $400 million!
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/125dd908-320d-400a-a77f-75cda1ee0161)


## Revenue
Revenue was analyzed based on genres and ratings. Following were the conclusions:

### Genres
1. Adventure movies were the highest grossing movies amongst all the genres:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/8045d542-3d00-4bb9-83c2-9e805dc9a653)

2.Target audience for adventure movies belong to the PG category:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/a788633c-23af-4a00-92a8-afc6b4157254)

### Ratings
1. PG-13 was the highest grossing movie category:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/4cf76b37-adcd-4476-a533-8cfb1f99c1ec)

2. In the PG-13 category, Action movies proved to be the most popular:
![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/853dba49-81fa-4556-9e6c-208460ec5488)

   
# Overall Conclusions
1. The studio should be looking at producing *Adventure* and *Action* movies catering to *PG* and *PG-13* audiences respectively.
2. Budgets for each genre can be expected to be around $50 million.
3. Although there are other factors in play, production budgets play a significant role in box-office returns i.e. bigger budgets may result in higher returns.


# Web Scraping 
Since the lack of good quality data was a major stumbling block, we can turn to scraping data from websites to gather better quality data. [Box Office Mojo](https://www.boxofficemojo.com/year/world/?ref_=bo_nb_in_tab) provides revenue information. By scraping data that spans 47 years, i.e. 1977-2023, we can see how web scapring can be useful when looking for quality data:

![image](https://github.com/rahulakrish/movie_studio_recommendation/assets/108379254/4c828963-c9c4-4e58-aadc-56e7de5a4907)



    
  


# Conclusion
By figuring out the largest market and the genres of movies that are most successful in the same, I can recommend to Microsoft Studio the kinds of movies that they should look to be producing and their target audience.

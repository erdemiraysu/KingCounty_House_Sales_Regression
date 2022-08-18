*** TO BE UPDATED ***

# MOVIE INVESTIGATIONS FOR MICROSOFT
***
## Overview
This project analyzes movie data to provide insights and recommendations about the kind of movies Microsoft should make for their new movie studio.

## Business Problem
***
What type of movies should Microsoft create?

 * Find a way to assess movie “profitability”.
 * Explore characteristics of past movies in relation to profitability: 
     - What genres of movies to make?
     - Which directors to work with?
     - When to release the movie?
     - Which movie length to focus on?

## Data
***
In the folder [zippedData](https://github.com/erdemiraysu/Movies_EDA_Project1/tree/master/zippedData) you will see:
* A dataset from IMDb which involves 4 tables and 140416 Distinct Movies representing movie characteristics such as `genre`, `year`, `runtime`, `director`.
* A dataset from The Numbers which involves `production_budget` as well as `gross` information of 5698 distinct movies

## Methods
*** 
* Derive **profit** (cost minus budget) and **return on investment** (profit/cost times 100) as means to assess "profitability". 
* Use **median** instead of mean as a measure of central tendency due to the skewness of the distributions and the high number of outlier movies.

## Results and Conclusions
***
WHAT GENRES OF MOVIES TO MAKE?

![Barplot_RoiProfitbyBudget_2](https://user-images.githubusercontent.com/61121277/168383501-2cf90adf-e46c-496d-9473-1c8780c64e19.png)
![Barplot_RoiProfitbyBudget_4](https://user-images.githubusercontent.com/61121277/168383513-2550647a-884c-44f8-b8e2-a1de2718af9f.png)
* With low budget ($4.5-16M), make movies of **Mystery** and **Horror**. They bring more than **300%** ROI and **$25-30M** in profit.
* With high budget (>$40M), make movies of **Animation**, **Adventure** and **Sci-Fi**. They bring close to **200%** ROI but **$200-250 M** in profit.

***
WHICH DIRECTORS TO WORK WITH?
![Barplot_Directors](https://user-images.githubusercontent.com/61121277/168383578-ed3cf70f-d2df-4c83-86b8-075fb6c94617.png)
For highest ROI and Profit invest on **James Wan, Pierre Coffin, Chris Renaud, Bryan Singer**.

***
WHEN TO RELEASE THE MOVIE?
![Barplot_ReleaseMonth](https://user-images.githubusercontent.com/61121277/168383553-23486525-573f-40b4-8be1-aa25035d1172.png)
* For highest ROI and profit release the movie in **November**. Skip December and next good option is **January**. 
* **Summer months** are also an option. 

***
HOW LONG SHOULD THE MOVIE BE?
![Barplot_RuntimeMinutes](https://user-images.githubusercontent.com/61121277/168383948-23831d24-eb6c-4a90-9a31-584de37f5d91.png)
For the highest Roi and Profit as well as the least risk target **120-160 min** length. This is  a bit longer than 2 hours. 

## Limitations and Improvements
***
* Small sample size - due to lack of budget and gross information. Perform API calls or wed scraping to increase sample size. 
* Movie names not coded the same way in different datasets - perform a more rigorous cleaning.
* Gather more information about Microsoft’s allocated budget to be able to provide more sensitive suggestions.

***
* The full analysis is in the [jupyter notebook](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/MovieProject_Notebook.ipynb). The pdf version of the same notebook is [here](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/MovieProject_Notebook.pdf). 
* Summary of the main findings are in the [presentation](https://github.com/erdemiraysu/Movies_EDA_Project1/blob/master/Presentation.pdf). 

## Repository Structure
    .
    ├── images 
    ├── zippedData 
    ├── MovieProject_Notebook.ipynb     
    ├── MovieProject_Notebook.pdf 
    ├── presentation.pdf                                             
    ├── README.md 
    └── movie_data_erd.jpeg   


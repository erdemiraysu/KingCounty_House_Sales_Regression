# KING COUNTY HOUSE REGRESSION
***
## Overview
This project analyzes house sale data from King County WA to provide insights and recommendations about the kind of houses "We Buy Ugly Houses" should invest on for their business.  

## Business Problem
***
We Buy Ugly Houses is a real estate investor (House Flipper) thay operates in King County WA. They purchase properties with the intention of remodeling to add value, then resell those properties for a profit. They want to know what type of houses to invest on for higher profit.

## Data
***
King County House Sales dataset is in the folder [Data](https://github.com/erdemiraysu/KingCountySales_Regression_Project2/tree/master/data). It contains house sale prices for King County sold between May 2014 and May 2015.

The variables/features included in the dataset are:

* `id` - Unique identifier for a house
* `date` - Date house was sold
* `price` - Sale price (prediction target)
* `bedrooms` - Number of bedrooms
* `bathrooms` - Number of bathrooms
* `sqft_living` - Square footage of living space in the home
* `sqft_lot` - Square footage of the lot
* `floors` - Number of floors (levels) in house
* `waterfront` - Whether the house is on a waterfront
* `view` - Quality of view from house
* `condition` - How good the overall condition of the house is. 
* `grade` - Overall grade of the house. Related to the construction and design of the house.
* `sqft_above` - Square footage of house apart from basement
* `sqft_basement` - Square footage of the basement
* `yr_built` - Year when house was built
* `yr_renovated` - Year when house was renovated
* `zipcode` - ZIP Code used by the United States Postal Service
* `lat` - Latitude coordinate
* `long` - Longitude coordinate
* `sqft_living15` - The square footage of interior housing living space for the nearest 15 neighbors
* `sqft_lot15` - The square footage of the land lots of the nearest 15 neighbors

## Methods
*** 
* Clean the dataset.
* Conduct feature engineering on the variables. 
* Build a series of linear regression models to come up with the best model to describe the relationship between the independent variables and the target/dependent variable (`house price`). 
* Check the linear regression assumptions to make sure normality, homoscadescacity are not violated and multicollinearity is not present.
* Draw conclusions and make suggestions about the kind of houses to invest on. 

## Results, Conclusions and Recommendations
![TornadoPlot_Coefs](https://user-images.githubusercontent.com/61121277/186974673-9d880bbc-a3b7-4e77-8844-730837e03823.png)
* The final model has an R-squared value of 0.753 means that the dependent variables explain 75% of the variability/change in price. 
* `Square footage of the house` is the most important variable to impact house price.  

***
![sqft_living_sqft_lot](https://user-images.githubusercontent.com/61121277/186549050-edb3140c-e940-4867-bdc5-9cdb50c099ec.png)
* Invest on increasing the total **square footage of the house** as much as possible (more than investing on the **lot size**). Every other feature kept constant, for every **1000** sqft increase in the house size, price increases by about **22%**.

***
![waterfront _to_Price](https://user-images.githubusercontent.com/61121277/186548886-b6f08e50-cff4-4b0c-8f14-1903a592ff2b.png)
* Being on **waterfront** increases the house price by **68%**, so invest on houses on waterfront. 

***
![month_price-relationship](https://user-images.githubusercontent.com/61121277/186548930-9b33a51c-1ec1-4798-96a9-bbaba72b7e2b.png)
* Put the house on the market in **April** which increases the price by **6.98%** if sold, compared to winter-fall or summer. The next best month is **March** with a **5.6%** increase. 

***
![LocationMap](https://user-images.githubusercontent.com/61121277/186548975-4db5078c-bd32-41c9-84a5-5201c2c2c74a.png)
* Invest on houses in **Seattle** area for **70%** increase in price, and **Medina, Bellevue, Mercer Island or Kirkland** for a 62% increase compared to the South.

## Limitations 
***
* Skewed data required outlier removal or data transformation.
* Zipcodes could not be used in regression due to the large number of levels (70)
* City to zipcode mapping did not work due to the zipcode and city boundaries overlapping.
 

## Improvements
***
* Clustering zipcodes into meaningful groups would be helpful.
* Gathering more detailed location info using API calls would enrich the modeling process.

***
* The full analysis is in the [jupyter notebook](https://github.com/erdemiraysu/KingCountySales_Regression_Project2/tree/master/Notebook.ipynb)

* The pdf version of the same notebook is [here](https://github.com/erdemiraysu/KingCountySales_Regression_Project2/tree/master/Notebook.pdf). 

* Summary of the main findings are in the [presentation](https://github.com/erdemiraysu/KingCountySales_Regression_Project2/tree/master/Presentation.pdf). 

## Contact Info:
* Email: erdemiraysu@gmail.com
* GitHub: @erdemiraysu
* [LinkedIn](linkedin.com/in/aysuerdemir/)

## Repository Structure
    .
    ├── images 
    ├── data 
    ├── KingCountySales.ipynb     
    ├── KingCountySales.pdf 
    ├── Presentation_KingCountySales.pdf                                             
    └── README.md   


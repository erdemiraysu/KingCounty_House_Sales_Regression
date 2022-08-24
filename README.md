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
* Build a series of linear regression models to come up with the best model to describe the relationship between the independent variables and the target/dependent variable (`house price`). 
* Check the linear regression assumptions to make sure normality, homoscadecity are not violated and multicollinearity does not present.
* Draw conclusions and make suggestions about the kind of houses to invest on. 

## Results and Conclusions

***
![sqft_living_sqft_lot](https://user-images.githubusercontent.com/61121277/186287087-e670c50b-cae7-4ef3-b8b3-84fde0550442.png)
* Invest on increasing the total **square footage of the house** as much as possible (rather than investing on the **lot size**). Every other feature kept constant, for every **1000** sqft increase in the house size, price increases by about **22%**.

***
![view_waterfront _to_Price](https://user-images.githubusercontent.com/61121277/186290603-ac13b86d-bd46-4d1b-9eda-27ea75c56912.png)
Being on **waterfront** increases the house price by **67%**, so invest on houses on waterfront. 

***
![month_price-relationship](https://user-images.githubusercontent.com/61121277/186287778-89776392-5e72-46e4-a99a-f0d95cfeb8a4.png)
* Put the house on the market in **April** which increases the price by **6.8%** compared to winter-fall or summer. The next best month is **March** with a **5.6%** increase. 

***
![LocationMap](https://user-images.githubusercontent.com/61121277/186287329-6817dec1-a8bd-4d6b-b1b3-01578f44e9fd.png)
Invest on houses in **Seattle** for **70%** increase in price, and **Medina, Bellevue, Mercer Island or Kirkland** for a 62% increase compared to the South.

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
    ├── data 
    ├── student.ipynb     
    ├── student.pdf 
    ├── presentation.pdf                                             
    └── README.md   


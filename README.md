# Food Sales Predictions

## An analysis of how certain factors within a relatively large grocery conglomerate affected the sales of different food items.

## Author: Joseph Lim

### Business Problem: 
Do any of the collected variables have a correlation with the sales of individual products within this businesses' stores? Can we predict the price of future food items based off of collected variables?

### Data:
The data consisted of 8523 rows, and 12 columns as listed in the data dictionary below. Data was provided via Coding Dojo's Part Time Data Science program, and originally came from [Analytics Vidhya's Big Mart Sales Practice Problem](https://https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

| Variable Name             | Description                                                                                         |   |   |   |
|---------------------------|-----------------------------------------------------------------------------------------------------|---|---|---|
| Item_Identifier           | Unique product ID                                                                                   |   |   |   |
| Item_Weight               | Weight of product                                                                                   |   |   |   |
| Item_Fat_Content          | Whether the product is low fat or regular                                                           |   |   |   |
| Item_Visibility           | The percentage of total display area of all products in a store allocated to the particular product |   |   |   |
| Item_Type                 | The category to which the product belongs                                                           |   |   |   |
| Item_MRP                  | Maximum Retail Price (list price) of the product                                                    |   |   |   |
| Outlet_Identifier         | Unique store ID                                                                                     |   |   |   |
| Outlet_Establishment_Year | The year in which store was established                                                             |   |   |   |
| Outlet_Size               | The size of the store in terms of ground area covered                                               |   |   |   |
| Outlet_Location_Type      | The type of area in which the store is located                                                      |   |   |   |
| Outlet_Type               | Whether the outlet is a grocery store or some sort of supermarket                                   |   |   |   |
| Item_Outlet_Sales         | Sales of the product in the particular store. This is the target variable to be predicted.          |   |   |   |

### Methods

#### Data Cleaning
* During the process of data cleaning, a large number (< 50%, > 25%) of rows were determined to be missing data. Sci-Kit Learn's SimpleImputer was used on the training data set in order to prevent data leakage. 

* Certain nominal categories could be considered ordinal (Outlet_Establishment_Year, Outlet_Size, Outlet_Location_Type). I chose to change Outlet_Establishment_Year into a string literal, so that the algorithms I used would not categorize them as numbers. For the Outlet_Size and Outlet_Location_Type, I was informed by an instructor that they did not seem to have a correlation and therefore could be deleted. While I chose to keep the columns, I have yet to corroborate this (see: Limitations & Next Steps).

#### Regression Analysis
* r^2 and RMSE were used to analyze regressions, as they provided a good base to judge the coefficient of determination as well as what the greatest variation was between experimental an actual results.

### Results

### Model

### Recommendations

The storeowner should focus on the last and most correlatable factors that impact food sales, specifically whether to stock items with higher_MSRP.

### Limitations & Next Steps
More EDA should be run on this data set in order to provide graphs that are more pleasing to the eye, as well as providing more visuals to choose from, and prove/disprove the usefulness of various columns as features within the test/train set.

### For further information

Please send me an email @ jplim96@gmail.com. 

### Overall time worked:
Approximately 10 hours of work went into this project. The project was started on 12/14/2022, and was finished on 2/3/2023. Roughly one hour per week was put into the project.

# Sales Predictions & Insights
# Analyzing Outlets and Outlets Types by Item Sales
Zach Dawson
When managing a business, often it is hard to keep track of sales when handling multiple stores. Predicting how certain types of stores with in you business can also be troubling to find out which type of store is producing the most sales.
### Data Source:
Big Mart Sales Predicition https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/
### Data Dictionary

|Variable Name	| Description |
|---------------|-------------|
| Item_Identifier |	Unique product ID |
|Item_Weight |	Weight of product |
|Item_Fat_Content |	Whether the product is low fat or regular |
|Item_Visibility |	The percentage of total display area of all products in a store allocated to the particular product |
|Item_Type |	The category to which the product belongs |
|Item_MRP |	Maximum Retail Price (list price) of the product |
|Outlet_Identifier |	Unique store ID |
|Outlet_Establishment_Year | The year in which store was established |
|Outlet_Size |	The size of the store in terms of ground area covered |
|Outlet_Location_Type |	The type of area in which the store is located |
|Outlet_Type |	Whether the outlet is a grocery store or some sort of supermarket |
|Item_Outlet_Sales |	Sales of the product in the particular store. This is the target variable to be predicted.  |

### To prepare the data, the data was cleaned, and the following processes proceed:
#### Exploratory Data Analysis
- During the exploratory data analysis, I created a histogram and a boxplot was created to compare two outlets.

<p align = "center">
  <img src = "https://github.com/zeekwired/sales-predictions/blob/main/outlet%202.png">
</p>
This is a histogram that shows two outlets that compare outlet item sales.

### Expanatory Data Analysis
- To help visualize the expanatory data, one bargraph and one histogram were chosen.
- The bargraph shows categories of outlets compared to each other.
- The histogram shows catergoies of outlets types compared to each other.

<p align = "center">
  <img src = "https://github.com/zeekwired/sales-predictions/blob/main/Outlet.png">
</p>
- Item Total Sales for Each Oulet: visualization to compare oulets by total sum of item outlet sales.
Top 3 highest earning Oulets:
- `OUT027` - $3,453,926.05
- `OUT035' - $2,268,122.94
- 'OUT049' - $2,183,969.81

Bottom 3 lowest earners:
- `OUT018` - $1,851,822.83
- `OUT010` - $188,340.17
- `OUT019` - $179,694.09

<p align = "center">
  <img src = "https://github.com/zeekwired/sales-predictions/blob/main/Item%20Sales.png">
</p>
- Item Total Sales by Outlet Type: histogram of counts of item outlet sales by outlet types.
Leading outlet:
  - `Supermarket Type3`
Lowest outlet:
  - `Grocery Store`
  
  ### Machine Learning Modules Used:
  - Linear Regression Model
  - Decision Tree Regressor Model
  
### Models Evaluation & Results:
- Linear Regression Model
    - Train MAE: 848.4782727267757
    - Test MAE: 803.9041870315474
    - Train MSE: 848.4782727267757
    - Test MSE: 1190756.9881949665
    - Train RMSE: 1141.36
    - Test RMSE: 1091.21
    - Train R2: 0.55
    - Test R2: 0.56
 
- Decision Tree Regressor Model
    - Train MAE: 762.6548715934737
    - Test MAE: 738.4803177114884
    - Train MSE: 762.6548715934737
    - Test MSE: 1118206.8715903033
    - Train RMSE: 1082.6553744791681
    - Test RMSE: 1057.4530115283153
    - Train R2: 0.6039330279227335
    - Test R2: 0.5947024005843626
    
- The choosen model was `Decision Tree Regressor Model`.
- For the testing set, 0.59% of the variance in y was explained by X.
- The Mean Absolut Error was off by $738.48
- The Mean Squared Error was $1,118,206.87
- The Root Mean Squared Error calculated $1057.45
Using this model would not be perferred considering the prediction that it created. Taking in consideration of the regression metrics from the models performance, there is a discrepancy between the R2 values and the Root Mean Squared. Also, the Mean Squared Error is too high to consider predicting with this model.

## Recommendations
Item Sales Insights
- Item sales for outlets and by types can help you achieve maxium effiency with item sales.
- By look at outlet types and what item MRP have you can deteremine what types should open in certain area's and what items have a better selling point.

Model Performance
- Overall, the best model in this analysis would have to be `DecisionTreeRegression`. There is still some basis affecting the models prediction, but it outperforms the `LinearRegression` model by far.
## Limitations & Next Steps
Now, I will continue forming this analysis to make it suitable for real world application. This is a starting point as in the future I will be dealing more with models and visualiztions like these.
## For Further Information
Contact information for questions:
- Zach Dawson
- zachd4145@gmail.com

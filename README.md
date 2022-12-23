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
#### Visualization Data Analysis
- During the exploratory data analysis, I created a histogram and a boxplot was created for categorical and number columns.

<p align = "center">
  <img src = "https://github.com/zeekwired/sales-predictions/blob/main/outlet%202.png">
</p>
This is a histogram that shows two outlets that compare outlet item sales.

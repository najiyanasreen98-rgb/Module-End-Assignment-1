Imported the data set to power query
In customer table found some inconsistent data in customer id and fixed them by find and replace .
sorted in ascending order, trimmed and cleaned, removed the duplicates if have any.
.In city column trimmed capitalized and cleaned to remove the inconsistent city names.
Followed the same steps in country column and state column as well.
Replaced the null rows with Unknown in Loyalty column. 
.In product table,Cleaned and Trimmed .sorted in ascending order.
removed the subcategory column
found the null values in the Cost which replaced by Median and changed the data type in to whole number.
.null values in the stock replaced by the median after replacing by custom column in Quantity ,total sales and unit price
formulas used for the discount column custom =if [Discount]=null then (Total amount /([quantity ]*[unit price]))-1
derived another customs from this formula
cleaned and trimmed the columns
In sales table order date column transformed to DMY format and price and sales column in to currency format
after transformations loaded to excel and connected each table by XLOOKUP function in a new sheet named final sales .
from this table created 4 pivot tables ,1.sales by region and store ,this table compares total sales across different regions and stores
2.sum of quantity by category and brand ;compares the number of products sold based on brands and category.3.cost by brand and category ;compares the production cost based on brand and category .4,revenue by brand and customer; shows which brand have high demand based on the customer loyalty type.
from the pivot tables created the pivot charts , styled  and designed .
added slicers based on category ,product id,region and category
pasted the charts and tables to the dashboard sheet created in next sheet .designed and arranged the dashboard as requirement and added 3 KPIs total sales ,total quantity and total cost .arrenged the slicers and connected to each table using report connections. 

# Keith-s-Electronics-Sales-Analysis-
The project involves exploratory data analysis to derive critical business insights that can help Keith’s Electronics improve its business. In this analysis, the sales data for 2019(January 2019 to December 2019) has been used to derive the aforementioned business insights.

Main Libraries Used During this Project
•	Pandas
•	Matplotlib
•	OS
•	Itertools
•	Collections

Data Description
As mentioned before, the data was for the year 2019 from January to December, and this data was combined and transformed in Excel before the analysis in Python. In Excel, null and duplicate values were removed, and the “Order Date” was converted to DATETIME, whereby the month was retrieved from the “Order Date” into a new column month. In total, the data has seven columns and over 180,000 rows. The following are the questions that guided data analysis.
Main Questions

Question 1: What was the best month for sales? How much was earned in that month?
This question was solved by first adding the sales column for every product and then using the “group by” function to group the sales according to the 12 months. 
December was the best month, with Sales of $4,613,443.34.
 

Question 2: What City had the highest number of Sales?
To answer this question, the first step was to create a city column, and after that, the (str.strip()) method was used to retrieve the cities from the “Purchase Address” column. It was essential to include the state of each City, considering that some states have similar city names, avoiding similar from being viewed as duplicates.
San Francisco is the City with the most sales: $8,262,203.91.


Question 3: What time should we display advertisements to maximize the likelihood of customers buying a product?
Using the (str.strip()) method, the time for each order was also retrieved from the “Order Date” column, but the only exception is that the time column was only filled with the hour each order was filled, as it is more viable as compared to using the overall time, i.e., (0830hrs).
Therefore, the best times to advertise are before 1100 hrs (11 am) and 1900 hrs (7 pm), as these times generate the most sales.
 

Question 4: What Products are most often sold together?
This problem was solved by grouping the “Order ID” while referencing the “Product” Column. These were the primary two columns used in this question, housed by a new data frame. After that, the libraries of itertools and collections helped to remove duplicates from the grouped columns and identified the most common products sold together.
Identifying the products that are most often sold together can help create promotions and sell them in bundles to increase sales.

The following were the results.
Product 1	Product 2	Count
iPhone	Lightning Charging Cable	1005
Google Phone	USB-C Charging Cable	987
iPhone	Wired Headphones	447
Google Phone	Wired Headphones	414
Vareebadd Phone	USB-C Charging Cable	361
iPhone	Apple Air pods Headphones	360
Google Phone	Bose SoundSport Headphones	220
USB-C Charging Cable	Wired Headphones	160
Vareebadd Phone	Wired Headphones	143
Lightning Charging Cable	Wired Headphones	92


Question 5: What product sold the most? Why do you think it sold the most?
This question was sold using the (group by) method, whereby the “product” column was grouped while referencing the sum of the “Quantity Ordered” column. This returned the results of the product with the most sales. To explain why most products had high numbers, a side-to-side comparison of sales and price was done to establish that the most sold were the cheapest.
Thus, the most sold products are AA Batteries(4-pack) at 27,635 units and AAA Batteries(4-pack) at 31,017 units. 
 


Reference
Keith Galli’s YouTube tutorials inspired this project.
- [Keith Galli’s YouTube Channel] (https://www.youtube.com/@KeithGalli)


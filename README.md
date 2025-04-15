# Amazon Sales Analysis


## Dataset Overview

The dataset used for this report is Amazon Sales dataset. It was obtained from Kaggle, a public website (https://kaggle.com). The dataset provides detailed insights into Amazon sales data including SKU code, design number, stock, category, size and colour. With this dataset, one can obtain information on which products sell best, which SEO titles generate the most sales and the best price range for a product in a category. 

This dataset consists mainly of categorical type of data which include Category: Type of product (String), Size: Size of the product (String), Status: Status of the sale (String), Fulfilment: Method of fulfilment (String), Style: Style of the product (String), SKU: Stock Keeping Unit (String), ASIN: Amazon Standard Identification Number (String), Courier Status: Status of the courier (String), Currency: The currency used for the sale (String), and B2B: Business to business sale (Boolean).
There are two numerical variables in the dataset; Qty: Quantity of the product (Integer) and Amount: Amount of the sale (Float). Date: Date of the sale (Date) is a temporal variable with time-related information.

## Dataset cleaning

Below is a screenshot of the raw dataset:

![Fig  1 1 Raw dataset](https://github.com/user-attachments/assets/95af9aa0-f73a-439e-a286-4e925045f934)


The following steps were carried out to clean the data:
- The dataset was checked for duplicates but no duplicates were found.
- Blank cells from the data were removed and headers made clear.
- 'Currency' and 'Ship-country' columns were removed.
- Rows with null in the 'Amount' column were removed.
- Rows with null in the 'Courier status' column were removed.

After cleaning the dataset, it consists of 116044 rows and 21 columns. Below is a screenshot of the clean dataset:

![Fig  1 2 Clean dataset](https://github.com/user-attachments/assets/874f6b1d-45ea-4b89-ae9f-7d9ff94705e9)



## DATA ANALYSIS AND VISUALISATION

### 1. Quantity by Week and Category

![Quantity by week and category](https://github.com/user-attachments/assets/d1552c74-7d9b-461d-9985-1f0d369f9456)

This is a bar chart showing quantity of clothing sold per week and category with ‘week’ on the x-axis and ‘quantity’ on the y-axis, ‘category’ is shown with colour indicators in each bar. The height of each bar corresponds to the total quantity of products sold for a particular category in the given week. The highest quantity of dresses sold was recorded on the week of April 18, 2022 while the lowest quantity was recorded on the week of June 27, 2022. The colour-coded bars can be used to quickly assess the performance of different product categories over time. It can be easily identified that the ‘set’ category consistently contributed the most to overall sales volume and the ‘kurta’ category exhibited fluctuations in demand.

### 2. B2B sales quantity

![B2B sales quantity](https://github.com/user-attachments/assets/7c3a9d0c-0971-4466-86df-3ce4c066c46e)

This circle chart illustrates B2B (business to business) sales quantity. The bigger circle depicting false is 99.28%, meaning that this percentage of sales was not from business but from individual consumers. The smaller circle depicting true is 0.72%, which means that 0.72% sales was from business. This information can be used to determine how to improve marketing efforts within a particular target audience.









### 3. Quantity by Status



This is a horizontal bar chart depicting the quantity of sales by courier status. The twelve courier statuses are on y-axis while quantity is on x-axis. Each bar represents a specific status such as ‘shipped’, ‘cancelled’, and ‘pending’ with the length of the bar indicating the quantity of sales associated with each status. The longest bar is that of status ‘shipped’ with 77,835 quantity of sales. Status ‘Shipped-Delivered to buyer’ has 28,879 quantity of sales. This shows that less than half of products shipped were eventually delivered to the buyer.


![Quantity by Status](https://github.com/user-attachments/assets/2c8db703-f1d4-46ec-80ae-b30d4b120fc8)




### 4. Quantity by Size and Category


This horizontal bar chart presents the quantity of sales across different product categories, segmented by size. The y-axis represents the different sizes while the x-axis represents the quantity of products sold. Bars within each size are colour-coded to represent different product categories. The bar chart shows that large size is the most popular within the ‘western dress’ product category, medium size is the most popular for ‘set’ category and large size is the most popular among buyers of the ‘kurta’ category. In total, medium size has the highest quantity in sales followed by large size. 


![Quantity by size and category](https://github.com/user-attachments/assets/e6e46a32-df28-4037-a421-b90f9caa17a3)






### 5. Quantity by Courier Status


This pie chart illustrates the distribution of sales quantity based on different courier statuses. It provides a concise summary of the proportion of sales orders categorised by their respective courier statuses. There are two courier status: shipped and unshipped. The size of each pie segment corresponds to the proportion of sales orders attributed to that particular courier status.  The larger segment (shipped) indicates a higher quantity of orders (109,896) with that status while the smaller segment (unshipped) indicates a lesser quantity of orders (6,586) with the status. This proportion of courier status gives an insight into the overall performance of the courier services utilised. Customers can be rest assured of receiving their orders with the obvious 94.35% success rate in shipping.

![Quantity by courier status](https://github.com/user-attachments/assets/b07cb3af-a3a6-4074-bac0-eafac380568d)




### 6. Quantity by Size of ethnic wear



It is a horizontal bar chart illustrating the quantity of ethnic wear according to their sizes. The clothes are grouped into two by ethnicity - Indian wear and others. The most ordered Indian wear is in size L (large), closely followed by size XL (extra large).The least ordered Indian wear is the free size. For the other category, the most ordered non-Indian wear is in size M (medium).







### 7. Top 10 states by quantity and category for ship-service level

![Top 10 states by quantity and Category for Ship- service level](https://github.com/user-attachments/assets/dddfb393-4ffc-421f-a566-c55746f3a711)


The horizontal bar chart shows quantity on the x-axis and ship-service level on the y-axis for the top 10 states. There are two ship-service levels: Expedited and Standard, each represented by its own colour code. Expedited ship service refers to shipping that delivers goods faster than the standard period of time. The graph shows that for all the top 10 states, expedited ship service is used more to deliver goods than the standard ship-service.












### 8. Amount by Week and Category


This line chart depicts the amount (price) of sales over time, organised by weeks, and segmented by different product categories. It provides a visual representation of how sales revenue fluctuates across various categories over time. The individual colours of each line represents category while each point on a line represents the amount (price) in a particular week. The ‘set’ clothing category recorded the highest sales revenue across all the weeks with the highest amount being INR3,691,013 on the week of May 2, 2022.

![Amount by week and Category](https://github.com/user-attachments/assets/af2815f6-0261-4601-9efb-71dada7a3b28)







### 9. Quantity by SKU and Category



SKU is Store Keeping Unit alphanumeric code used for tracking a product in sales. The chart is a horizontal bar chart showing quantity by SKU. The product with SKU JNE3797-KR-L which is the code for ‘Western dress’ has the highest quantity in sales of 661.












### 10. Quantity by Promotion-IDs by Category



This is a horizontal bar chart depicting the quantity of category products sold on the x-axis and the promotion IDs on the y-axis. Promotion IDs are unique codes used to run promotion campaigns on products. The promotion ID with the highest quantity is [IN Core Free Shipping 2015/04/08 23-48-5-108]. This visualization can be used to track the effectiveness of promotion campaigns.






## DATA MINING

### Implementation of data mining algorithm:

- The csv format of the dataset was imported into Weka.
- The data was pre-processed.
- J48 classifier was created in Weka, default parameters were used.
- The decision was generated and visualised to understand the rules used to classify different room types.
- The accuracy of the generated model was tested using the “percentage of correctly predicted instances” and “confusion matrix” as metrics.

First iteration: 





There are 122100 instances with 21 attributes. The attributes are: index, order ID, date, status, fulfilment, sales channel, ship-service-level, style, SKU, category, size, ASIN, courier status, quantity, amount, ship-city, ship-state, ship-postal-code, promotion-ids, B2B, and fulfilled-by. 99.91% instances were correctly classified during cross-validation and 0.089% instances were incorrectly classified.















Second iteration after removing the following variables: fulfilment and fulfilled by.




There are 19 attributes. The correctly classified and incorrectly classified instances remained the same.99.91% instances were correctly classified during cross-validation and 0.089% instances were incorrectly classified.


Third iteration after removing order id, sales channel and ASIN:



There are 16 attributes. 99.91% instances were correctly classified and 0.089% were incorrectly classified during cross validation. This means that the ability of the model to make accurate predictions remained the same.


## CONCLUSION

### Overall Visualisation results

- The highest volume of sales was from individual customers
- Higher volume of orders are shipped and people place their orders using expedited shipping more than standard ship
- Western dress has the highest sales even though the 'set' category sold more consistently across a long period. 
- Generally, medium and large sizes were highly ordered. 
- Non-indian wear was sold in higher quantities than Indian wear.

 ### Data Mining results

- The data mining algorithm used is Decision trees - J48
- The confusion matrix showed a high number of true positives and true negatives, which is a good indication that the model is a good fit for the data.
- The 1st iteration was chosen because the stability of the model suggests convergence meaning that the tree has reached a point where splitting the data further will not lead to better accuracy.
- It has 99.91% correctly classified instances. 

### Business Intelligence obtained from results

1. Amazon should focus on promoting the sale of dresses in the weeks of low sales to increase revenue.
2. As the majority of sales are from individual consumers, the business can research ways to attract and retain business clients to increase B2B sales.
3. Shipped status has the highest quantity of sales, the business should prioritise efficient shipment and delivery to make sure that shipped orders are delivered to the customers.
4. Clothing in medium and large sizes should be produced more than other sizes due to their higher sales quantity while adjusting inventory for less popular smaller sizes.
5. The company can consider placing more stock in size L for Indian wear to cater to customer needs and increase sales.
6. Western dress and  'set' wear should be produced more to cater to the needs of customers.
7. Amazon should  keep track of the effectiveness of promotion campaigns and adjust based on their impact on sales quantity. 




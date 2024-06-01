<h1 align="center"> Information About Dataset </h1>

<br>

- Dataset :

      - 2022 (March, April, May, June, July, August)

# This file contains all the Table information regarding the columns described in the CSV files.
1. dim_customers.csv
2. dim_products.csv
3. dim_date.csv
4. dim_targets_orders.csv
5. fact_order_lines.csv
6. fact_orders_aggregate.csv

<br>


## 🔶 Column Description for  "dim_customers":
This table contains all the information about customers

1. customer_id: Unique ID is given to each customer
2. customer_name: Name of the customer
3. city: It is the city where the customer is present


<br>
<br>



## 🔶 Column Description for  "dim_products":
<img align="center" src = "https://github.com/Manish7272/Supply-Chain-Optimization-Project-Manager/assets/71213166/4da465b4-4678-46dc-9532-92baa19b1879">

This table contains all the information about the ***products***
1. product_name: It is the name of the product
2. product_id: Unique ID is given to each of the products
3. category: It is the class to which the product belongs


<br>

We have 3 FMCG Products in this Dataset:
- 1.Dairy = AM Milk [100, 250, 500] ,  AM Butter [100, 250, 500], AM Ghee [100, 150, 250], AM Curd [50, 100, 250]

- 2.Food = AM Biscuits [250, 500, 750]

- 3.Beverages = AM Tea [100, 250, 500]

<br>
<br>

## 🔶 Column Description for  "dim_date":
This table contains the dates at daily, monthly level and week numbers of the year

1. date: date at the daily level
2. mmm_yy: date at the monthly level
3. week_no: week number of the year as per the date column

<br>

## 🔶 Column Description for  "dim_targets_orders":
This table contains all target data at the customer level

1. customer_id: Unique ID that is given to each of the customers
2. ontime_target %: Target assigned for Ontime % for a given customer
3. infull_target %: Target assigned for infull % for a given customer
4. otif_target %:   Target assigned for otif % for a given customer

<br>

## 🔶 Column Description for  "fact_order_lines":
This table contains all information about orders and each item inside the orders.

1. order_id: Unique ID for each order the customer placed
2. order_placement_date: It is the date when the customer placed the order
3. customer_id: Unique ID that is given to each of the customers
4. product_id: Unique ID that is given to each of the products
5. order_qty: It is the number of products requested by the customer to be delivered
6. agreed_delivery_date: It is the date agreed between the customer and Atliq Mart to deliver the products
7. actual_delivery_date: It is the actual date Atliq Mart delivered the product to the customer
8. delivered_qty: It is the number of products that are actually delivered to the customer


<br>

## 🔶 Column Description for  "fact_orders_aggregate":
This table contains information about  "OnTime",  "InFull"  and "OnTime Infull"  information aggregated at the order level per customer

1. order_id: Unique ID for each order the customer placed
2. customer_id: Unique ID that is given to each of the customers
3. order_placement_date: It is the date when the customer placed the order
4. on_time: '1' denotes the order is delviered on time. '0' denotes the order is not delivered on time.
5. in_full: '1' denotes the order is delviered in full quantity. '0' denotes the order is not delivered in full quantity.
6. otif:    '1' denotes the order is delviered both on time and in full quantity. '0' denotes the order is either not delivered on time or not in full quantity.

<br>
<br>

## Model View:
![Screenshot 2024-01-28 194704](https://github.com/Manish7272/Supply-Chain-Optimization-Project-Manager/assets/71213166/3e138654-a850-4af6-9a4c-d08f3ccf5973)

<br>
<br>
<br>

![Screenshot 2024-01-29 020641](https://github.com/Manish7272/Supply-Chain-Optimization-Project-Manager/assets/71213166/0cc067ab-438a-44f4-8467-b71cce96e14c)

<br>
<br>
This was a Challenge put up by a famous YouTuber Codebasics and he provided all the datasets. This time no mock up was provided. Instead we got a conversation between the stakeholders of the company with their Data Analyst. From that conversation we had to figure out the requirements needed to solve the supply chain problem. We had to create a dashboard which showed the overall insights to the stakeholders and also give us enough insights to help solve the supply chain problem. #codebasicsresumeprojectchallenge

<br>


<br>

# 𝐏𝐫𝐨𝐛𝐥𝐞𝐦 𝐒𝐭𝐚𝐭𝐞𝐦𝐞𝐧𝐭:
A few key customers haven't renewed the annual contract due to the service issues. This might have resulted in the bad service experience. Hence, the managenent wants to track the "On-Time" & In-Full" delivery service levels for all the customers on daily basis to fix them and later expand the business to new cities.

# Amazon_Vine_Analysis

## Deliverable 1: Perform ETL on Amazon Product Reviews

<img width="1413" alt="Screen Shot 2022-04-25 at 8 17 00 PM" src="https://user-images.githubusercontent.com/93845867/165206467-ad526d43-51bf-49bd-9df9-ffae8ad4ea79.png">

<img width="1270" alt="Screen Shot 2022-04-25 at 7 03 38 PM" src="https://user-images.githubusercontent.com/93845867/165206509-9311862e-dbc0-4309-895f-749e425dda77.png">

<img width="1275" alt="Screen Shot 2022-04-25 at 7 06 19 PM" src="https://user-images.githubusercontent.com/93845867/165206525-283538b5-8872-43fc-9241-5b7ff4d50d8b.png">

## Deliverable 2: Determine Bias of Vine Reviews

<img width="1414" alt="Screen Shot 2022-04-25 at 8 18 01 PM" src="https://user-images.githubusercontent.com/93845867/165206580-e5d621cb-0b41-42ee-bea7-780cf35b861f.png">

<img width="1411" alt="Screen Shot 2022-04-25 at 8 18 44 PM" src="https://user-images.githubusercontent.com/93845867/165206594-c2683c6a-7c48-454f-9950-ea6c362c3119.png">

## Deliverable 3: A Written Report on the Analysis (README.md)

### Overview of the analysis: Explain the purpose of this analysis.

I picked one of the Amazon beauty datasets and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I uses PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

### Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?

- Paid: 647 
- Unpaid: 74,113  

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- Paid: 229  
- Unpaid: 43,217 

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- Paid: 35.394126738794434  
- Unpaid: 58.312306882733125 

### Summary: 

I believe this particular category is popular enough to not have to rely heavy on paid Vines. Popularity and quality of products seem to speak for themselves. Additionaly, the majority of paid reviews weren't 5-star rated, which makes me believe that they were paid for by competing companies in an attempt to smear reputation of rival products. 
One additional analysis we can do to support my statement is to find mean, median and mode for paid and unpaid Vines. 

# Amazon Vine Analysis

## Overview

This project conducts an analysis of the Amazon Vine program, which is a service that allows manufacturers and publishers to receive reviews for their products. The analysis focuses on a specific dataset containing reviews of products in the "Video Games" category. The goal is to determine if there is any bias towards favorable reviews from Vine members (who are paid for their reviews) compared to non-Vine members.

## Data Source

The dataset used for this analysis is sourced from the Amazon Review datasets available on the AWS public dataset repository. Specifically, the dataset contains reviews of products in the "Video Games" category.

## Tools and Technologies Used

- Python
- PySpark
- Amazon Web Services (AWS)

## Methodology

1. **Data Preparation**: The dataset is loaded and preprocessed using PySpark to extract relevant information such as product ratings, helpful votes, and Vine membership status.

2. **Analysis**: The dataset is analyzed to compare the ratings and helpfulness of reviews between Vine and non-Vine members. Statistical metrics such as average rating and percentage of helpful votes are calculated for each group.

3. **Results Interpretation**: The results of the analysis are interpreted to determine if there is any significant difference in review characteristics between Vine and non-Vine members.

## Key Findings

- Average rating: The average rating given by Vine members is compared to that of non-Vine members to assess any potential bias.
- Percentage of helpful votes: The percentage of helpful votes received by reviews from Vine members is compared to that of non-Vine members to evaluate reviewer credibility.

## Conclusion

Based on the analysis results, conclusions are drawn regarding the presence of bias in reviews from Vine members compared to non-Vine members. Recommendations may be provided for further investigation or action based on the findings.

## Repository Contents

- **Data**: Contains the dataset used for the analysis.
- **Notebooks**: Includes Jupyter notebooks containing the Python code for data preprocessing, analysis, and visualization.
- **Results**: Contains any visualizations or summary reports generated from the analysis.
- **References**: Includes any relevant literature or documentation used as references for the analysis.

## Usage

To replicate the analysis, follow these steps:

1. Clone the repository to your local machine.
2. Install the necessary dependencies (PySpark, etc.).
3. Open and run the Jupyter notebooks in the "Notebooks" directory sequentially to preprocess the data, conduct the analysis, and generate results.

## Credits

The dataset used for the analysis is sourced from the Amazon Review datasets available on the AWS public dataset repository.

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

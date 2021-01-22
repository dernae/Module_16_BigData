# Module_16_BigData

## Overview 

The purpose of this project is to analyze the responses of the participants of members of the paid Amazon Vine program.
Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. The reviews 
are incentivized by companies like SellBy that pay a small fee to Amazon and provide products to Amazon Vine members. 
The analysis was conducted on reviews of furniture attained from https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt 
I usedd PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and 
load the transformed data into pgAdmin. I continued to use PySpark to determine if there is any bias toward favorable reviews 
from Vine members in your dataset.

### Customers' Table Output on pgAdmin
<br><br>
![](https://github.com/dernae/Module_16_BigData/blob/main/postgres%20outputs/customers_table_output.PNG)<br>

### Product Table Output on pgAdmin
![](https://github.com/dernae/Module_16_BigData/blob/main/postgres%20outputs/products_table_output.PNG)<br>

### Reviews Table Output on pgAdmin
![](https://github.com/dernae/Module_16_BigData/blob/main/postgres%20outputs/review_data_table_output.PNG)<br>

### Response Table Output on pgAdmin
![](https://github.com/dernae/Module_16_BigData/blob/main/postgres%20outputs/vine_table_output.PNG)<br>
## Results 
- There were 17,490 non-Vine reviews and 8,082 of them were 5-stars.
- The percent ratio of paid vs unpaid reviews fell somewhere around 0.8%.
## Summary 

The numbers indicate that there is a low occurence of positivity bias. Additional future analysis could include running a similar 
analysis across the board and determining which category is more prone to positivity bias. 

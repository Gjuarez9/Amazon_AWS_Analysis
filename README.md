# Amazon "VINE" Reviews; Analysis

### Overview

The purpose of this analysis was to use Amazon reviews written by members of their paid Amazon Vine program, and then determine if there is any bias toward favorable reviews from Vine members in the given dataset.

The dataset I used contained revews for mobile apps and was provided on amazons aws https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

The tools I used to execute this analysis were Google Colab, Amazon AWS, PostgreSQL, VS Code, PySpark, GitHub & GitBash.

### Results

After extracting my dataset from the Amazon AWS servers I extracted the required data and created four dataframes that would allow me to get the required information into tables.

The tables were the following
  - "customers_table"
  - "products_table"
  - "review_id_table"
  - "vine_table"
  
They were created in order to get a allow for deeper exploration into each table feature. In order to use them I creaded an Amazon Web Services RDS instance and connected it to my PostgreSQL server. An example query after succesful linkage can be seen bellow.

SQL_Query.png

https://github.com/Gjuarez9/Amazon_AWS_Analysis/blob/main/Resources/SQL_Query.png



### Summary

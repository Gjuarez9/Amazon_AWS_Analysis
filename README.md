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

![SQL_Query](https://user-images.githubusercontent.com/107452167/194994113-7a3b8e89-a948-4ac1-ada1-db3525d569e3.png)

I then used PySpark to dive deeper into the review data

### Summary

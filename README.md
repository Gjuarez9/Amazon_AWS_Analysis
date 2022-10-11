# Amazon "VINE" Reviews; Analysis

### Overview

The purpose of this analysis was to use Amazon reviews written by members of their paid Amazon Vine program, and then determine if there is any bias toward favorable reviews from Vine members in the given dataset.

The dataset I used contained revews for mobile apps and was provided on amazons aws [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt).

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

I then used PySpark to dive deeper into the review data & create new dataframes for specific requests.

* Find the total number of revews
* Find total number of paid reviews and the percentage that was 5 stars
* Find total number of unpaid reviews and the percentage that was 5 stars

Coincidentally for my dataset the number of unpaid reviews was the same as the number of total reviews (meaning there were no paid reviews) 129,516

![Unpaid](https://user-images.githubusercontent.com/107452167/194996765-1a74e4fb-8f74-40fb-abc7-f8090dbe3b94.png)

The total paid five star reviews were 0 & percentage of unpaid five star reviews was 0% as well.

![Paid](https://user-images.githubusercontent.com/107452167/194998963-a7766311-db8c-495c-89aa-8f3a1c5b7da3.png)

The total unpaid five star reviews were 59,278 & percentage of unpaid five star reviews was 45.76%

![percents](https://user-images.githubusercontent.com/107452167/194996888-6ab24f7e-6cbd-4b4a-9f6d-07d0a5302cf1.png)

### Summary

With the little ammount of information that I was able to gather it is hard to make a concrete conclusion into the analysis. However I think that the fact that 45.76% of 5 star reviews in the vine program are unpaid we can assume that there isn't really a bias or if there is there is a light one. That is due to individuals perhaprs rating a certain app highly due to the fact that they are hoping to perhaps become paid members. On the other hand you can say that they simply just enjoy the product and there isn't a correlation between the two.We can explore this deeper by looking into the conversion rate of members going from unpaid to paid reviewees as well as look into why there are no paid five star reviews in our app. That could also just mean that none of the paid reviewers liked the product enough to rate it that well.

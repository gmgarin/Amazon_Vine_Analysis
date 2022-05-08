# Amazon_Vine_Analysis

## Overview of the analysis:

### This project aims to analyze Amazon reviews written by members of the paid Amazon Vine Program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. In this project, a data set was selected from a pool of datasets. Each dataset contains reviews of specific product. Video games products reviews was selected for this particular analysis. 

### The analysis performed involved the ETL process to extract the dataset, trasform the dataset , and connect to an *Amazon Web Services RDS* instance, and loaded the transformed data into *pgAdmin*. After which, further analysis was done using *PySpark*, *Pandas*, and *SQL* to determine if there is any bias toward favorable reviews in the selected dataset.

## Results:

### The selected dataset has approximately 1.8 million reviews. These data were transformed and filteredinto a DataFrame as shown below:

<p align="center">
   Extracted Data transformed into DataFrame
</p>

![This is an image](https://github.com/gmgarin/Amazon_Vine_Analysis/blob/8febc4db4c1849e54396ebee34d11c31302007a3/Resources/image1.png)

<p align="center">
   Filtered DataFrame
</p>

![This is an image](https://github.com/gmgarin/Amazon_Vine_Analysis/blob/1f61989655a8b7a72b04cc1f3a28fd4439d534e5/Resources/image2.png)

### After filtering and transforming the extracted dataset that contains 1.8 million reviews, the following results were obtained:
- There are 94 Vine reviews and 15, 663 non-Vine reviews.
- There are 48 five-star Vine reviews and 15, 663 five-star non-Vine reviews.
- 51.1% of Vine reviews are five-star while 38.7% accounts for five-star ratings for non-Vine reviews.




## Summary:
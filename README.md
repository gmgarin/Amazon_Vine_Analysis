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

<p align="center">
   Summarized Data
</p>

![This is am image](https://github.com/gmgarin/Amazon_Vine_Analysis/blob/2b3e05990e7fd6610e5e86d1e4cf22ce8ee74476/Resources/image4.png)



## Summary:

### After careful analysis, it can be inferred that Vine members tend to show bias when rating video game products. The majority (51%) of all the ratings by Vine members are five-star. On the other hand, non-Vine members tend to give less than five-star ratings as only 39% of non-Vine reviews are five-star. However, it should be noted that there is huge difference between each sample sizes (94 Vine reviews vs 40,471 non-Vine reviews). To make a more sound and conlusive comparative analysis as to which group tend to show bias, the difference between sample sizes of the two groups should be at minimum. Furthermore, additonal analysis can be done such as comparing average Vine five-star ratings across all categories versus average non-Vine five-star ratings across all categories. 
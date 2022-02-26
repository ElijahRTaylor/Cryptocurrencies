# Cryptocurrencies



## Overview
In an effort to classify different cyptocurrencies by their features, we will use an unsupervised machine learning model to group the different cryptocurrencies into clusters.  

To achieve this, we will do the following:

1.Preprocess the Data for PCA
2.Reduce Data Dimensions Using PCA
3.Cluster Cryptocurrencies Using K-means
4.Visual Cryptocurrencies Results
## Results

### Preprocess the Data for PCA

For this step, we preprocess the data to ensure that there out model does not get unneccesary input and that everything is formatted in a usable form.  We remove rows with NaNs, we change certain fields to binary values, and we remove columns that are not necessary.

### Reduce Data Dimensions Using PCA

We then us PCA to reduce the dimensions to 3 principal components.

![Screen Shot 2022-02-26 at 12 59 27 AM](https://user-images.githubusercontent.com/87248687/155831531-88e57ce0-d6e9-4ae9-9ea4-6013d28cafae.png)


### Cluster Cryptocurrencies Using K-means

Using the K-means algorithm, we created an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame.  We then ran the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.


![Screen Shot 2022-02-26 at 1 03 47 AM](https://user-images.githubusercontent.com/87248687/155831658-b978705b-9b3a-4354-8a6c-c53fa1e70e1d.png)

### Visual Cryptocurrencies Results

For this step, we visualized the distinct groups that correspond to the three principal components and then we created a table with all the currently tradable cryptocurrencies.


![Screen Shot 2022-02-26 at 1 07 04 AM](https://user-images.githubusercontent.com/87248687/155831781-66ba3fb2-f9e6-4198-9b46-fdfc406e3b69.png)



![Screen Shot 2022-02-26 at 1 08 07 AM](https://user-images.githubusercontent.com/87248687/155831872-a6f3e9f6-18d9-4046-bb94-63ea83266328.png)


## Summary

For the most part, the majority of the cryptocurrencies appear to belong to either class 0 or class 1.  We would probably have to look further into some of the things cryptocurrencies in these classes have in common.

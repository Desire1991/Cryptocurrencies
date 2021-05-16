# Cryptocurrencies

## Overview of Analysis


A cryptocurrency is a digital or virtual currency that is secured by cryptography, which makes it nearly impossible to counterfeit or double-spend. Many cryptocurrencies are decentralized networks based on blockchain technology, a distributed ledger enforced by a disparate network of computers. A defining feature of cryptocurrencies is that they are generally not issued by any central authority, rendering them theoretically immune to government interference or manipulation


For this cryptocurrencies analysis I created a report that includes which cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. The data source that we are working with is not ideal, so we needed a process to fit the machine learning models. Since there is no known output, unsupervised learning would be the most logical method of machine learning. To group the cryptocurrencies, I used a clustering algorithm and data visualizations to share the findings.


## Results


First, I used the Pandas library to process the dataset in order to perform the Principal Component Analysis (PCA) algorithm. Then I applied the Principal Component Analysis (PCA) algorithm, and reduced the dimensions of the x DataFrame to three principal components and placed the dimensions in a new DataFrame. Using the K-means algorithm, I created an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame. Then, I ran the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. Finally, I created scatter plots with Plotly Express and hvPlot to visualize the distinct groups, then created a table with all the currently tradable cryptocurrencies using the hvPly.table() function.

## Elbow Curve
<img width="780" alt="Screen Shot 2021-05-15 at 10 15 07 PM" src="https://user-images.githubusercontent.com/74233163/118384518-314cba80-b5cc-11eb-8d7a-569dcd6c951f.png">


## 2D Scatter Plot
<img width="738" alt="Screen Shot 2021-05-15 at 10 14 46 PM" src="https://user-images.githubusercontent.com/74233163/118384520-36116e80-b5cc-11eb-9f2b-691f9110af7f.png">


## 3D Scatter Plot
<img width="835" alt="Screen Shot 2021-05-15 at 9 53 58 PM" src="https://user-images.githubusercontent.com/74233163/118384533-4e818900-b5cc-11eb-9a4e-6dba2afc761f.png">


## Tradable Cryptocurrencies Table
<img width="727" alt="Screen Shot 2021-05-15 at 10 14 06 PM" src="https://user-images.githubusercontent.com/74233163/118384535-55100080-b5cc-11eb-8f5f-09cae3efc3b8.png">

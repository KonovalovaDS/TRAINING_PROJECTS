# <p align="center"> RFM Analysis

<p align="center"><img src = https://www.marketing91.com/wp-content/uploads/2018/11/What-is-RFM-Analysis-1024x576.jpg></p>

## <p align = "center"> Customer Segmentation in E-Commerce

## Content
[1. Project description](README.md#project-description)

[2. Dataset](README.md#dataset)

[3. Conclusion](README.md#conclusion)

[4. Contacts](README.md#contacts)

### Project description

**Business target**:
Make the segmentation of existing customers, analyse these segments and determine the strategy for interacting with them.

**Technical task**:
Build the model of customer clustring based on their purchasing power, order frequency and the time since the last purchase, and determine the profile of each cluster.

**Main goals**:

- Preprocess the dataset;
- Conduct EDA and identify key patterns;
- Form product and customer categories;
- Build several machine learning models that solve the problem of customer clustering, determine the number of the clusters and interpret them;
- Design the process for predicting the category of customer interests and test the model for new customers.

[To the top](README.md#content)

### Dataset

The dataset can be found following the link: https://drive.google.com/file/d/1Dqgs5jN7PKplodiV94UkTkuYXbhVdnC-/view?usp=sharing

The dataset contains more than half a million transactions, each of which is described by the following features:

- **InvoiceNo** - invoice number (a unique six-digit nominal number assigned to each transaction; the letter "C" at the beginning of the code indicates a cancellation if the transaction);
- **StockCode** - product code (a unique five-digit integer assigned to each individual product);
- **Description** - product name;
- **Quantity** - quantity of each product per transaction;
- **InvoiceDate** - invoice / transaction date and time;
- **UnitPrice** - unit price in British pounds;
- **CustomerID** - customer identifier (a unique five-digit number uniquely assigned to each customer);
- **Country** - name of the country in which the customer resides.

[To the top](README.md#content)

### Conclusion

Due to the large amount of entries, the following dimensionality reduction techniques were used:

- Principal Component Analysis (PCA); and
- t-Distributed Stochastic Neighbor Embedding (t-SNE)

The following clustering methods were applied:

- K-Means Clustering;
- Gaussian Mixture Model; and
- Agglomerative Clustering.

Based of sulhouette score the optimal number of clusters were used in the best possible algorithm. The achieved results are:

**<p align="center"> PCA reduced data**

|**Method**|**Silhouette Score**|**Number of Clusters**|
|:--|:--|:--|
|K-Means|0.52|3|
|GaussianMixture|0.44|3|

**<p align="center"> t-SNE reduced data**

|**Method**|**Silhouette Score**|**Number of Clusters**|
|:--|:--|:--|
|K-Means|0.4816|8|
|GaussianMixture|0.4688|4|
|AgglomerativeClustering|0.479|8|

In order to predict the clusters for new customers the Random Forest Classifier and Gradient Boosting Classifier were used. Both models showed almost the same result: 0.989 and 0.988 respectively, although maximum depth were significantly different 14 and 6 accordingly. Therefore Gradient Boosting is more efficient.

[To the top](README.md#content)

### Contacts

*<p align="center">[Email](natalia_konovalova@icloud.com)</p>*

*<p align="center">[LinkedIn](https://www.linkedin.com/in/natalia-ds-198612241)</p>*

*<p align="center">[YouTube](https://www.youtube.com/@DsCsheets)</p>*

[To the top](README.md#content)
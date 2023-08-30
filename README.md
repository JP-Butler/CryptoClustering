
# Module 19 - Unsupervised Learning

  

## Crypto Clustering Challenge
In this challenge I used my prior Python knowledge acquired in previous modules and newly gained ***Unsupervised Learning*** concepts to predict if and how various cryptocurrencies are affected by 24-hour or 7-day changes. To analyze these phenomenon Python's extensive Machine Learning library `scikit-learn` was used along with 2 algorithms: an algorithm `KMeans` that clusters data into seperate samples of equal variance and `PCA` a statistical technique that streamlines the machine learning process by reducing the number of features used for the clustering. 
  
  

## Table of Contents

  

- [About & Process](#about--process)

- [Getting Started & Installing](#getting-started--installing)

- [Resources](#resources)

- [Contributing](#contributing)

## About & Process
This project was broken down into 7 sections, as follows: <br>
1. **Prepare the Data**
Where I used the `StandardScaler()` to normalize the data and created a new dataframe to store the scaled data.
2. **Find the Best Value for k Using the Original Scaled DataFrame**
I created 2 lists, 1 for the k values and another empty one for the inertia values. A for loop to find the inertia, assign them to the k values  and append to the inertia list. A dictionary to store the above data, and finally plot the data into a *Elbow Curve* line chart to analyze. 
3. **Cluster Cryptocurrencies with K-means Using the Original Scaled Data**
This section is where I defined my KMeans model, trained it with `.fit()` and made predictions with `.predict()`to finally create cluster predictions with the original scaled data. Finally plotting into a scatter plot to visualize the clusters.
4. **Optimize Clusters with Principal Component Analysis**
Using the original scaled data I performed a PCA to reduce the features to 3 principal components. Used `.explained_variance_ratio()`to see how much info can be attributed to each principal component. And formed the new PCA values into a DataFrame for further analysis later.
5. **Find the Best Value for k Using the PCA Data**
Here I repeated section 2 but this time with the PCA data instead, to see how reducing the features affects the k-values and what the optimal value is. 
6. **Cluster Cryptocurrencies with K-means Using the PCA Data**
Like section 5, in this section we repeat section 3 using the PCA data this time. To visualize how the reducing the features to cluster affects the actual clustering. 
7. **Visualize and Compare the Results**
Finally, 2 composite plots are created. 1 to compare the two Elbow Curve line plots, and another the compare the two Clustering scatter plots. 
  

## Getting Started & Installing

A few libraries are needed to run the code file:

* `pandas`, see the [Anaconda Download](https://www.anaconda.com/distribution/#windows) site to install the full python package, Anaconda is a distribution of Python and should bring in all python libraries when completed.

* `scikit-learn`, Python's Machine Learning library. Run the following in your terminal if needed:
`conda install scikit-learn `


## Resources

* Composite plots `hvplot` documentation: [Composite Plots](https://holoviz.org/tutorial/Composing_Plots.html)
* `scikit-learn` Clustering Documentation [scikit-learn.org](https://scikit-learn.org/stable/modules/clustering.html)


## Contributing

  

Justin Butler

  

**Aided By:**  <br>

* class Teacher's Assistant

* Weekly Tutoring session

> Written with [StackEdit](https://stackedit.io/).
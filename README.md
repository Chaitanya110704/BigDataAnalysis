# Big-Data-Analysis

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*:CHAITANYA NAMDEO

*INTERN ID*:CT04DL130

*DOMAIN*:DATA ANALYTICS

*DURATION*:4 WEEKS

*MENTOR*:NEELA SANTHOSH 

*Description of the Dask-based Iris Dataset Analysis Script*
This Python script demonstrates scalable data analysis using the Iris dataset and Dask, a parallel computing library. It follows these steps:
1.Load Dataset: Uses scikit-learn to load the built-in Iris dataset into a pandas DataFrame and adds species names as a categorical column.
2.Simulate Large Data: Repeats the dataset 10,000 times to simulate a large dataset (~1.5 million rows).
3.Convert to Dask DataFrame: Converts the large pandas DataFrame to a Dask DataFrame with 10 partitions for parallel processing.
4.Data Analysis with Dask:
Counts the number of records per species.Calculates average feature values (sepal and petal dimensions) for each species.Generates summary statistics (mean, std, min, max, etc.) for the entire dataset.
5.Save Results: Writes the species counts, average features, and summary statistics to separate CSV files.
This script is useful for learning how to scale data analysis workflows using Dask, especially when working with datasets too large to fit into memory.

*OUTPUT*:
self._meta = self.obj._meta.groupby(
Species Count:
 species
setosa        500000
versicolor    500000
virginica     500000
dtype: int64

 self._meta = self.obj._meta.groupby(
Average Feature Values by Species:
             sepal length (cm)  sepal width (cm)  petal length (cm)  \
species                                                              
setosa                  5.006             3.428              1.462   
versicolor              5.936             2.770              4.260   
virginica               6.588             2.974              5.552   
          petal width (cm)  
species                       
setosa                 0.246  
versicolor             1.326  
virginica              2.026  

Summary Statistics:
        sepal length (cm)    sepal width (cm)   petal length (cm)  \
count       1.500000e+06      1.500000e+06       1.500000e+06   
mean        5.843333e+00      3.057333e+00       3.758000e+00   
std         8.253016e-01      4.344111e-01       1.759405e+00   
min         4.300000e+00      2.000000e+00       1.000000e+00   
25%         5.100000e+00      2.800000e+00       1.600000e+00   
50%         5.800000e+00      3.000000e+00       4.350000e+00   
75%         6.400000e+00      3.300000e+00       5.100000e+00   
max         7.900000e+00      4.400000e+00       6.900000e+00   
...

25%        3.000000e-01  
50%        1.300000e+00  
75%        1.800000e+00  
max        2.500000e+00 


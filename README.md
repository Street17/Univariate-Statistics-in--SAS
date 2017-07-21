
Hi folks!
This is my second series on SAS after fundamentals of SAS. In this post I will explain what all we shall keep in mind while summarizing all the aspects of a dataset.
Let us quickly go through the basis on which we can summarize our datasets and what all we need to remember while summarizing our datasets.
We can summarize our dataset on the following:-
•	Central Tendency (Average)
•	Variability
•	Shape
These summaries can be later presented as
•	Numerical Summary
•	Data Visualization
Note - I am assuming here you are familiar with the definition of mean, median and mode. 
To look at the short picture of numerical variables we should use mean or median and for categorical variables we should use mode. We shall never use mean as the representation of data when we have extremely high or low values.
In some cases it might happen that data set have same average like same mean or median we shall not consider the data sets to be same in these cases because it is possible that they differ in terms of spread (variability). For example, both the data sets shown below have average as 10
{7, 8, 9, 15, 11, 12, 13}: 10
{-200, 50, 10, and 90,100}: 10
Here second data is much more widely spread than first data set. We can measure the variability in the datasets by following measures:-
•	Range
•	Mean Absolute Deviation (MAD)
•	Standard Deviation (or Variance where Variance = (SD)^2)
•	Inter Quartile Range
Note - I am assuming here you are familiar with the definition of Range, Mean Absolute Deviation, Standard Deviation/Variance and Inter Quartile Range
In practice we use IQR as the measure of variability because it is not tedious to calculate like mean absolute deviation and standard deviation/variance and is not sensitive to extreme values like range in fact IQR is the one measure which is not sensitive to outliers even.
Given a sample value we can comment on its possibility of being from a dataset just by understanding the shape of the data set this is why it is important to understand the shape of the dataset. 
To get the idea about shape we generally use histogram or plot frequency bar charts. In practice there are three types of frequency distributions 
•	Normal (No skew)
•	Negatively Skewed
•	Positively Skewed

While summarizing our data set it is important that we keep outliers out of the picture. We can identify an outlier by defining out data set limits. We generally define the limit of dataset as 
[q1 -1.5*IQR, q3+1.5*IQR] or as 
[µ-k* σ, + µ k* σ] where, k is a real number and mostly taken as 2 or 3.
In industry we generally use the latter one. All the values beyond the limits should be treated as outliers.
So folks! That’s all for univariate statistics now let us see this practically in SAS. 

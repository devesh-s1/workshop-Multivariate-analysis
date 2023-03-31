# Workshop-Multivariate-analysis
## AIM
To perform Multivariate EDA on the given data set.

##Explanation Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

## Algorithm

## Step1
Import the built libraries required to perform EDA and outlier removal.

## Step2
Read the given csv file.

## Step3
Convert the file into a dataframe and get information of the data.

## Step4
Return the objects containing counts of unique values using (value_counts()).

## Step5
Plot the counts in the form of Histogram or Bar Graph.

## Step6
Use seaborn the bar graph comparison of data can be viewed.

## Step7
Find the pairwise correlation of all columns in the dataframe.corr()

## Step8
Save the final data set into the file.

## Types of bivariate analyis
1)Numerical & Numerical(Scatter plot)
2)Numerical & Categorical(Bar plot,Box plot,Dist plot)

## Code
```
Developed by : Devesh Sharma
Registration Number : 21222211008
```
```
import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()
```
## Output
## Data Head
![1](https://user-images.githubusercontent.com/121490523/229038376-a8ff2270-596d-4503-a392-fbcbe8af55e4.png)
## Data Information
![2](https://user-images.githubusercontent.com/121490523/229038476-02f124f2-5dff-4620-be68-9e7c971079fa.png)
## Numerical & Numerical(Scatter plot)
![3](https://user-images.githubusercontent.com/121490523/229038553-c4e811c3-b3bd-4492-a78b-2d55294a198b.png)
## Numerical & Categorical(Bar plot)
![4](https://user-images.githubusercontent.com/121490523/229038652-0ae83896-f398-4ef5-ac4d-15d5d26ea478.png)
## Non-Graphical method(correlation)
![5](https://user-images.githubusercontent.com/121490523/229038771-15bd0900-d31b-4208-af8e-6f5ed3abb092.png)
## Result
Thus we have performed Multivariate EDA on the given data set.

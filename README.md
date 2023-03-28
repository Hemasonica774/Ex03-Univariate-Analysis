
# Ex03-Univariate-Analysis

## AIM:

To read the given data and perform the univariate analysis with different types of plots.

## EXPLANATION:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# ALGORITHM:

##  Step1:

Read the given data.

## Step2:

Get the information about the data.

## Step3:

Remove the null values from the data.

## Step4:

Mention the datatypes from the data.

## Step5:

Count the values from the data.

## Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

# CODE:

## code 1:

```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
print(df)
df.head()
df.info()
df.dtypes
df.describe()
sns.boxplot(x='Postal Code',data=df)
sns.countplot(x="Postal Code",data=df)
sns.histplot(x="Postal Code",data=df)
df.skew()
sns.boxplot(x="Sales",data=df)
sns.histplot(x='Postal Code',data=df)
sns.displot(x="Postal Code",data=df)
df.kurtosis()
sns.boxplot(x="Sales",data=df)

```

## code 2:

```

import pandas as pd
import seaborn as sns
df1=pd.read_csv("diabetes.csv")
print(df1)
df1.info()
df1.dtypes
df1.skew()
df1.describe()
sns.boxplot(x='Glucose',data=df1)
sns.countplot(x="Glucose",data=df1)
sns.displot(df1["Glucose"]) 
sns.histplot(x="Glucose",data=df1)
df1.skew()
df1.kurtosis()
sns.boxplot(x="Insulin",data=df1)

```

# OUTPUT:

DATA

![image](https://user-images.githubusercontent.com/118361409/228319191-76c48776-a6ac-49ce-97a0-50c871738640.png)

DATA HEAD
![image](https://user-images.githubusercontent.com/118361409/228319348-d7757085-44fb-46b3-bf88-41a3bad09e39.png)

DATA INFORMATION

![image](https://user-images.githubusercontent.com/118361409/228319575-9a7aeb37-0025-4ed8-bee2-b3c6a311758f.png)

DATA DESCRIBE

![image](https://user-images.githubusercontent.com/118361409/228319783-db993ea2-af24-4202-8b25-183e603a83cf.png)

BOXPLOT

![image](https://user-images.githubusercontent.com/118361409/228320203-115c3223-511a-4b66-a06e-20f673751c82.png)


COUNTPLOT

![image](https://user-images.githubusercontent.com/118361409/228320648-13880383-c59c-4969-977d-383517f12544.png)

HISTROGRAM PLOT

![image](https://user-images.githubusercontent.com/118361409/228321005-92ff8a25-5ccb-479c-a6fb-b5ecb82a6728.png)

SKEW

![image](https://user-images.githubusercontent.com/118361409/228323878-83077ce3-1078-4673-8b47-bf1267e1cfa0.png)


BOXPLOT


![image](https://user-images.githubusercontent.com/118361409/228322798-2582a520-5007-4959-8776-5f0fbc3c6892.png)


HISTROGRAM PLOT

![image](https://user-images.githubusercontent.com/118361409/228322937-6621c9fd-70b9-446e-a262-a487b293161f.png)


DISTRIBUTION PLOT


![image](https://user-images.githubusercontent.com/118361409/228323061-a0a12943-5042-4948-9c40-38713cbe0e0f.png)


KURTOSIS


![image](https://user-images.githubusercontent.com/118361409/228323252-4d53f757-e59f-4a13-a830-a8b5e4ee964e.png)


BOX PLOT

![image](https://user-images.githubusercontent.com/118361409/228323356-9316bbe4-45b7-4849-b38b-bd5567e9cf15.png)










# RESULT:

Thus the experiment completed sucessfully

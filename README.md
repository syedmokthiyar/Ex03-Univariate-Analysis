# Ex03-Univariate-Analysis

# Aim:

To read the given data and perform the univariate analysis with different types of plots.

# Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:

# Step1:

Read the given data.

# Step2:

Get the information about the data.

# Step3:

Remove the null values from the data.

# Step4:

Mention the datatypes from the data.

# Step5:

Count the values from the data.

# Step6:

Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:

# (1) Diabetes.csv

```py
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
sns.distplot(df["Glucose"])
sns.histplot(x="Glucose",data = df)
df.kurtosis()
sns.boxplot(x="Glucose",data=df)
```

# (2) SuperStore.csv

```python
df2 = pd.read_csv("/SuperStore.csv")
df2.head()
df2.isnull().sum()
df2['Postal Code'] = df2["Postal Code"].fillna(df2['Postal Code'].mode()[0])
df2.isnull().sum()
df2.dtypes
df2.describe()
df2['Sales'].value_counts()
sns.boxplot(x="Sales",data=df2)
sns.countplot(x="Sales",data=df2)
sns.distplot(df2['Sales'])
sns.histplot(x="Sales",data=df2)
df2.skew()
sns.distplot(df2["Postal Code"])
sns.histplot(x="Postal Code",data = df2)
df2.kurtosis()
sns.boxplot(x="Row ID",data=df2)
```

# OUTPUT:

# DIABETES.csv

![output](/1.png)

## INFO

![output](/2.png)

## ISNULL.SUM

![output](/3.png)

## DTYPES

![output](/4.png)

## DESCRIBE

![output](/5.png)

## VALUECOUNTS

![output](/6.png)

## BOXPLOT

![output](/7.png)

## COUNTPLOT

![output](/8.png)

## DISTPLOT

![output](/9.png)

## HISTPLOT

![output](/10.png)

## SKEW

![output](/11.png)

## DISTPLOT SKEW

![output](/12.png)

## HISTPLOT SKEW

![output](/13.png)

## KURTOSIS

![output](/14.png)\

## BOXPLOT KURTOSIS

![output](/15.png)

# SUPERSTORE.csv

![output](/a.png)

## ISNULL.SUM

![output](/b.png)

## AFTER CLEANING

![output](/c.png)

## DTYPES

![output](/d.png)

## DESCRIBE

![output](/e.png)

## VALUECOUNTS

![output](/f.png)

## BOXPLOT

![output](/g.png)

## COUNTPLOT

![output](/h.png)

## DISTPLOT

![output](/i.png)

## HISTPLOT

![output](/j.png)

## SKEW

![output](/k.png)

## DISTPLOT SKEW

![output](/l.png)

## HISTPLOT SKEW

![output](/m.png)

## KURTOSIS

![output](/n.png)

## BOXPLOT KURTOSIS

![output](/o.png)

# RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.

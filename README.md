### Ex03-Univariate-Analysis
### Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
### Step1:
Read the given data.

### Step2:
Get the information about the data.

### Step3:
Remove the null values from the data.

### Step4:
Mention the datatypes from the data.

### Step5:
Count the values from the data.

### Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

### Program:
DEVELOPED BY : HARINI.M.D

REG NO : 212222230043
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
### Output:
### Dataset:
![image](https://user-images.githubusercontent.com/113497680/228889573-50aae2d6-7f36-4811-81a3-029f49b813e0.png)
### Head:
![image](https://user-images.githubusercontent.com/113497680/228889973-09c0b10d-8d94-494c-98b0-b03004eb7371.png)
### Info:
![image](https://user-images.githubusercontent.com/113497680/228890615-ba23ac16-5072-4226-bc00-e9c58e8a9c5c.png)
### Describe:
![image](https://user-images.githubusercontent.com/113497680/228890855-15d4bd18-e50d-48fe-a361-e722f596cbcc.png)
### Isnull:
![image](https://user-images.githubusercontent.com/113497680/228891341-b5c1f4ea-bdfb-455b-a39f-38d420a1331e.png)
### Dtypes:
![image](https://user-images.githubusercontent.com/113497680/228891568-7829ed95-5a7a-4e09-bf31-b7009cd89108.png)
### Valuecount:
![image](https://user-images.githubusercontent.com/113497680/228891798-8c1b50b1-47ba-4f5a-ade1-7ea060abf07a.png)
### Boxplot:
![image](https://user-images.githubusercontent.com/113497680/228891921-4a8dccff-89d0-4d23-8de5-dac8ad231ecd.png)
### Countplot:
![image](https://user-images.githubusercontent.com/113497680/228892074-fdeb346f-1a34-486e-86e5-5df0f5b29b4a.png)
### Distribution plot:
![image](https://user-images.githubusercontent.com/113497680/228892246-cb5ba2ff-6cc6-4a9a-ac7d-52802b3cb315.png)
### Histogram plot:
![Uploading image.png…]()

### Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.



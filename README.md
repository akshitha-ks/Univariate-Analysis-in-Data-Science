AIM:
    To perform Univariate Analysis on the given data.
    
ALGORITHM:
       Step 1: Read the given data.
       Step 2: Get information from the data.
       Step 3: Perform the Univariate Analysis.
       Step 4: Save the clean data to the file.
       
CODE:

SuperStore.csv

import pandas as pd
import seaborn as sns
df=pd.read_csv("/content/SuperStore.csv")
df.isnull().sum()
df.info()
df.dtypes
sns.boxplot(x='Sales',data=df)
sns.countplot(x='State',data=df)
sns.displot(df["State"])
sns.histplot(x="State",data=df)
df.skew()

Diabetes.csv

import pandas as pd
import seaborn as sns
df=pd.read_csv("/content/diabetes.csv")
df.isnull().sum()
df.info()
df.dtypes
sns.boxplot(x='Age',data=df)
sns.countplot(x='Age',data=df)
sns.displot(df["Age"])
sns.histplot(x="Age",data=df)
df.skew()

OUTPUT:





RESULT:
         Univariate Analysis is performed on given data and save.

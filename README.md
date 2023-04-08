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

SuperStore.csv

![image1](https://user-images.githubusercontent.com/123535064/230724537-3f17dc9f-4f30-47a8-8977-00dbd56ec127.png)

![image](https://user-images.githubusercontent.com/123535064/230724584-1912ca9d-8246-4e8d-ae46-7d1a1ce03146.png)

![image](https://user-images.githubusercontent.com/123535064/230724610-26b5cf3c-76d2-4599-bef5-1dcec30de62d.png)

![image](https://user-images.githubusercontent.com/123535064/230724615-8498811c-2095-4554-ba46-3bd1c2d304aa.png)

![image](https://user-images.githubusercontent.com/123535064/230724619-781e646c-da94-4177-930f-a9daf19b35ea.png)

![image](https://user-images.githubusercontent.com/123535064/230724628-68cee9ad-a0c0-466f-8992-fbd525793a94.png)

![image](https://user-images.githubusercontent.com/123535064/230724632-b5c1af7c-10d6-4bba-b422-c148463484b1.png)

![image](https://user-images.githubusercontent.com/123535064/230724639-705cabb1-bc83-4e51-aea3-34ee8671568b.png)


diabetes.csv

![image](https://user-images.githubusercontent.com/123535064/230724663-2022e1af-b33a-4d4b-a836-c7c4f8c53b21.png)

![image](https://user-images.githubusercontent.com/123535064/230724673-f2084ac6-3513-44ab-acf8-598f199a11c9.png)

![image](https://user-images.githubusercontent.com/123535064/230724679-c60cd979-22c1-43c2-90d9-ceefac8f4fd4.png)

![image](https://user-images.githubusercontent.com/123535064/230724684-cca49210-b5ee-407a-a87d-3654a0ba9c7d.png)

![image](https://user-images.githubusercontent.com/123535064/230724690-27b81d74-cd88-45cf-8677-8ab0e3be6c38.png)

![image](https://user-images.githubusercontent.com/123535064/230724700-154d5d1f-030f-420e-9efe-a234b16d0f51.png)

![image](https://user-images.githubusercontent.com/123535064/230724709-b5002ae8-e802-4b3e-a436-6f8ed9942979.png)

![image](https://user-images.githubusercontent.com/123535064/230724727-1c4fd29b-17c0-497c-ae36-b7adf7954885.png)



RESULT:

         Univariate Analysis is performed on given data and save.

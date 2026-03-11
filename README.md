# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding :
Import Required Libraries:
````
import seaborn as sns
import pandas as pd

df=pd.read_csv("iris.csv")

df.head()

cor=df.corr(numeric_only=True)
cor

sns.heatmap(cor)

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='hex')

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='reg')

sns.pairplot(df)

sns.pairplot(df,hue='sepal_width')

sns.distplot(df['sepal_length'])

sns.distplot(df['sepal_length'],kde=False,bins=10)

sns.countplot(x='species',data=df)

sns.countplot(y='species',data=df)

sns.barplot(x='petal_length',y='petal_width',data=df)

sns.barplot(x='petal_width',y='petal_length',data=df)

sns.boxplot(x='species',y='sepal_width',data=df)

sns.boxplot(x='species',y='sepal_length',data=df,palette='rainbow')

sns.boxplot(data=df,orient='v',palette='rainbow')

sns.boxplot(x='sepal_length',y='sepal_width',hue='species',data=df)

sns.violinplot(x='sepal_length',y='species',palette='rainbow',data=df)

````
# Output:


<img width="527" height="418" alt="image" src="https://github.com/user-attachments/assets/e3c9adb1-b870-4c4d-a889-00109404f296" />


<img width="589" height="590" alt="image" src="https://github.com/user-attachments/assets/589d0184-f28a-4761-96e5-296bba807455" />


<img width="589" height="590" alt="image" src="https://github.com/user-attachments/assets/a1de9f5d-fbb6-438d-95ca-67cf4c88d6ed" />


<img width="986" height="986" alt="image" src="https://github.com/user-attachments/assets/5ad0c802-1dfc-448f-bf79-bbd1fc92be71" />

<img width="841" height="740" alt="image" src="https://github.com/user-attachments/assets/cd16a1e6-1766-418a-9744-eaac48aaedc4" />

<img width="567" height="433" alt="image" src="https://github.com/user-attachments/assets/b0b9d094-27f3-434c-8216-d35179871182" />


<img width="544" height="433" alt="image" src="https://github.com/user-attachments/assets/3e7105ec-879d-48c3-b360-1905d3e3dab1" />


<img width="562" height="432" alt="image" src="https://github.com/user-attachments/assets/736f30a8-7cc4-4f1d-80f1-9e012da49e9b" />


<img width="613" height="432" alt="image" src="https://github.com/user-attachments/assets/5c62b820-014d-406c-bfff-cb94fc759e5c" />



<img width="572" height="433" alt="image" src="https://github.com/user-attachments/assets/d59d2c9b-4079-47d4-9ffa-71dda31685d1" />



<img width="554" height="436" alt="image" src="https://github.com/user-attachments/assets/77c7aad1-03b5-46c9-a145-48a897a4b5d3" />


<img width="567" height="435" alt="image" src="https://github.com/user-attachments/assets/0429331f-823e-40d2-9103-9d335c974007" />


<img width="567" height="432" alt="image" src="https://github.com/user-attachments/assets/cc149d8a-4977-43b4-ad3d-a89f2e20187b" />


<img width="534" height="413" alt="image" src="https://github.com/user-attachments/assets/7a22016c-dfd6-477d-aed3-9577ef853a86" />



<img width="571" height="435" alt="image" src="https://github.com/user-attachments/assets/94473476-8b1c-41e4-9678-b936aa4e0a9c" />


<img width="613" height="433" alt="image" src="https://github.com/user-attachments/assets/a9c485de-ee87-49a1-b3df-839fcfd01a54" />



# Result:
Thus , The Data Visualization using Seaborn is Performed Successfully.

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

# Coding and Output:

import seaborn as sns

df=sns.load_dataset("iris")

df.head()

df.corr()

sns.heatmap(df.corr())

sns.jointplot(x='sepal_length',y='petal_length',data=df,kind='hex')

sns.jointplot(x='sepal_length',y='petal_length',data=df,kind='reg')

sns.pairplot(df)

sns.pairplot(df,hue='species')

sns.distplot(df['sepal_length'])

sns.distplot(df['sepal_length'],kde=False,bins=10)

## Count plot

sns.countplot(x='species',data=df)

## Count plot

sns.countplot(y='species',data=df)

## Bar plot
sns.barplot(x='sepal_width',y='species',data=df)

## Bar plot
sns.barplot(x='species',y='sepal_width',data=df)

df.head()

sns.boxplot(x='sepal_length',y='petal_length', data=df)

sns.boxplot(x="sepal_width", y="petal_length", data=df,palette='rainbow')

sns.boxplot(data=df,orient='v')

# categorize my data based on some other categories

sns.boxplot(x="petal_length", y="petal_width", hue="sepal_length",data=df)

sns.violinplot(x="sepal_width", y="species", data=df,palette='rainbow')

# OUTPUT:

<img width="790" height="627" alt="Screenshot 2026-03-09 111731" src="https://github.com/user-attachments/assets/ba2173dc-c7fa-46c6-b4e8-4cc3e244b476" />

<img width="721" height="734" alt="Screenshot 2026-03-09 111756" src="https://github.com/user-attachments/assets/a82a6736-6ad6-4a74-be36-f04b6ea01e3b" />

<img width="963" height="853" alt="Screenshot 2026-03-09 111819" src="https://github.com/user-attachments/assets/a90437f2-55ae-4046-975d-a7a648478a1c" />

<img width="591" height="450" alt="Screenshot 2026-03-09 111829" src="https://github.com/user-attachments/assets/11bd6b45-1f05-4ea0-9af8-38baf5857b56" />

<img width="585" height="448" alt="Screenshot 2026-03-09 111848" src="https://github.com/user-attachments/assets/0a9a9bb4-5bca-4f32-8e33-19740ebbe5f3" />

<img width="590" height="450" alt="Screenshot 2026-03-09 111914" src="https://github.com/user-attachments/assets/44d42fb5-5355-4aee-bcaf-7a27610ad31f" />

<img width="557" height="435" alt="Screenshot 2026-03-09 111940" src="https://github.com/user-attachments/assets/0a2dc814-68ef-4ccf-bb47-0543cee0f8ea" />

<img width="641" height="453" alt="Screenshot 2026-03-09 111957" src="https://github.com/user-attachments/assets/38c953a6-7b5e-4cf4-83cc-45e456f71ab4" />

# Result:
Thus, the Data Visualization using seaborn python library for the given data is successfully performed.

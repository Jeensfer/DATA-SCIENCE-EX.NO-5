# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import matplotlib.pyplot as plt
import pandas as pd
from sklearn.datasets import load_iris

# STEP 1: Load dataset
iris = load_iris()

# STEP 2: Convert to DataFrame
df = pd.DataFrame(
    iris.data,
    columns=iris.feature_names
)

# STEP 3: Visualize data

# Line Plot
plt.figure(figsize=(6,4))
plt.plot(df["sepal length (cm)"])
plt.title("Line Plot")
plt.xlabel("Index")
plt.ylabel("Sepal Length")
plt.show()


# Histogram
plt.figure(figsize=(6,4))
plt.hist(df["petal length (cm)"], bins=10)
plt.title("Histogram")
plt.xlabel("Petal Length")
plt.ylabel("Frequency")
plt.show()


# Scatter Plot
plt.figure(figsize=(6,4))
plt.scatter(
    df["sepal length (cm)"],
    df["petal length (cm)"]
)
plt.title("Scatter Plot")
plt.xlabel("Sepal Length")
plt.ylabel("Petal Length")
plt.show()


# Bar Plot
plt.figure(figsize=(6,4))
df.mean().plot(kind="bar")
plt.title("Average Feature Values")
plt.ylabel("Value")
plt.show()


# Box Plot
plt.figure(figsize=(6,4))
plt.boxplot(df["sepal width (cm)"])
plt.title("Box Plot")
plt.show()
```
<img width="694" height="394" alt="image" src="https://github.com/user-attachments/assets/e5f8a4b6-a6f7-4239-8012-c0e5a0856186" />
<img width="605" height="392" alt="image" src="https://github.com/user-attachments/assets/c240144f-03fd-425e-95f6-8df67f4ff5ab" />
<img width="543" height="393" alt="image" src="https://github.com/user-attachments/assets/da974ac1-af4d-4fb2-a7da-802dd9d5713b" />
<img width="573" height="483" alt="image" src="https://github.com/user-attachments/assets/81a4aa64-cc53-47b9-b334-05145b670302" />
<img width="534" height="376" alt="image" src="https://github.com/user-attachments/assets/223e73c4-fe03-410b-9f21-96b1b7be13bc" />


# Result:
 Include your result here

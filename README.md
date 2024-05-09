# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:


> Developed By: Shriram S

> REG NO: 212222240098
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/c81670c7-4750-41aa-a2d2-665c96dc791c)![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/1f56e035-35e4-4b5c-942e-e659713aa3de)


### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/9d490a21-08af-4a86-baba-0d666dfbb6bd)![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/e4fb55f1-5ac4-4ecf-b6b0-f9fcb2f193f9)


### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```


![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/730eb037-dd3b-4bf8-9b63-3fd6653cc5c3)![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/bd76a160-b8a5-4326-a898-5703d7a904f3)



### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/f2d9b5b2-31fe-49cb-beb8-c364fed293d2)



### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/e9b4561f-3ab2-4000-81e9-be4555b26d8e)



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```


![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/9a8a76fb-6c31-4fb9-a991-df97c6bdc09d)



### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/73c2e1c3-55a2-4a9c-ad8d-149efd550778)


```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![image](https://github.com/ShriramGH/EXNO-5-DS/assets/117991122/f13275ce-abe8-47f3-88eb-9c48d186a488)


## Result:

### Thus, all the data visualization techniques of matplotlib has been implemented.

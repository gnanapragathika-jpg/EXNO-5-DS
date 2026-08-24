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
import pandas as pd 
import numpy as np 
import seaborn as sns 
import matplotlib.pyplot as plt
```

## LINE PLOT:

```
marks=[13,45,63,78] 
student=['ABC','QOR','EFB','TOB'] 
plt.plot(marks,student) 
plt.xlabel('Marks') 
plt.ylabel('Student name') 
plt.show()
```

<img width="796" height="532" alt="image" src="https://github.com/user-attachments/assets/fcb4109d-20e7-4165-badc-5d493a5e7313" />

```
student=['A','B','C','D'] 
attendence=[90,85,73,88] 
plt.plot(attendence,student) 
plt.xlabel('Attendence') 
plt.ylabel('Student name') 
plt.show()
```

<img width="750" height="541" alt="image" src="https://github.com/user-attachments/assets/fb4bea86-cbe5-4f61-8a72-e2b5850443b0" />

## SCATTER PLOT:

```
x=[10,20,30,40,50] 
y=[100,200,300,400,500] 
plt.scatter(x,y,label='stars',color='green',marker='*',s=30) 
plt.show()
```

<img width="763" height="512" alt="image" src="https://github.com/user-attachments/assets/7eb4e652-d49a-4f56-9c68-67247cbd910f" />

```
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

<img width="795" height="552" alt="image" src="https://github.com/user-attachments/assets/5285c956-429a-4bf5-b078-3f7467caf6c1" />

## PIE CHART:

```
act=['eat','sleep','work','play'] 
slices=[3,7,8,6] 
color=['r','y','g','b'] 
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%') 
plt.legend() 
plt.show()
```

<img width="667" height="510" alt="image" src="https://github.com/user-attachments/assets/69df2cae-bee2-44f5-a858-aa72ceec7f57" />

```
feedback=['Good','excellent','Perfect','Ok'] 
slices=[4,10,3,8] 
color=['y','r','b','g'] 
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%') 
plt.legend() 
plt.show()
```

<img width="635" height="492" alt="image" src="https://github.com/user-attachments/assets/050aa10b-2b3b-42a1-b8e8-7e1da4c2f242" />

## AREA CHART:

```
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

<img width="758" height="502" alt="image" src="https://github.com/user-attachments/assets/10ba01a3-20e7-4be9-93c7-112acb526779" />

## BAR CHART:

```
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

<img width="863" height="562" alt="image" src="https://github.com/user-attachments/assets/629463c0-67c0-45d3-aeff-daeac2d77006" />

## HISTOGRAM:

```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x, bins = 10, color='blue', alpha=0.5) 
plt.show()
```

<img width="735" height="502" alt="image" src="https://github.com/user-attachments/assets/ef2cca4e-f5cf-4191-9a7a-c17b6f5bb63c" />

## BOX PLOT:

```
np.random.seed(0) 
data=np.random.normal(loc=0, scale=1, size=100) 
data
```

<img width="713" height="425" alt="image" src="https://github.com/user-attachments/assets/9101b410-8395-4532-a9fc-08a5c83df7dd" />

```
fig, ax= plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values') 
ax.set_title('Box Plot')
```

<img width="738" height="598" alt="image" src="https://github.com/user-attachments/assets/a23f57ae-ee19-42c2-ae01-f588b0551b58" />

## Result:

Thus,the given Data Visualization using matplot python library as executed successfully.

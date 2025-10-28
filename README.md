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
## Line Plot:

```
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
<img width="716" height="534" alt="image" src="https://github.com/user-attachments/assets/a090c4de-f8fd-4371-9c6f-fb3b05ce1d5a" />

<img width="688" height="541" alt="image" src="https://github.com/user-attachments/assets/bb57e09b-3a8f-493e-a25b-63df0bed9886" />

## Scatter Plot:

```
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
<img width="686" height="506" alt="image" src="https://github.com/user-attachments/assets/4fff9bac-4af2-4132-94be-9bfcd215d459" />

<img width="693" height="564" alt="image" src="https://github.com/user-attachments/assets/0e559054-ee81-43e8-899e-f03a1933bd0b" />

## Pie Chart:

```
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
<img width="558" height="514" alt="image" src="https://github.com/user-attachments/assets/6f51a142-cfdc-453d-9ef0-46a0dd114885" />

<img width="540" height="495" alt="image" src="https://github.com/user-attachments/assets/36e95c96-53ba-41d3-9712-e60055eec323" />

## Area Chart:

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
<img width="688" height="512" alt="image" src="https://github.com/user-attachments/assets/ea7b7f1e-6a2e-40ef-9210-b0079e73dbd9" />

## Bar Chart:

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
<img width="701" height="564" alt="image" src="https://github.com/user-attachments/assets/5c9361ba-7f1f-40c7-bf4a-c5efb896c875" />

## Histogram:

```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

<img width="663" height="511" alt="image" src="https://github.com/user-attachments/assets/d2619bc5-451e-44ae-b4ca-a00615e9c1b7" />

## Box Plot:

```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="879" height="445" alt="image" src="https://github.com/user-attachments/assets/660da882-2ba5-4405-8611-4db1e2b7845c" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="774" height="604" alt="image" src="https://github.com/user-attachments/assets/84bcf3ea-bc08-4285-b086-a2de7b4732af" />

# Result:

 Thus the program is executed successfully.

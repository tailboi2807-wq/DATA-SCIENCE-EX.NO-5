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
 ~~~
import pandas as pd 
import numpy as np 
import seaborn as sns 
import matplotlib.pyplot as plt 
#Line Plot: 
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
~~~
<img width="722" height="767" alt="image" src="https://github.com/user-attachments/assets/4e009538-a0c0-41b0-b1d4-84a0d67c7138" />


~~~
#Scatter Plot: 
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
~~~
<img width="587" height="732" alt="image" src="https://github.com/user-attachments/assets/ab596fb0-f4f2-42e0-9cfe-0236e3167e3c" />


~~~
#Pie Chart: 
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
~~~
<img width="581" height="690" alt="image" src="https://github.com/user-attachments/assets/749499d8-300b-4e78-9eeb-6e8ec8f5d7a7" />


~~~
#Area Chart: 
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
~~~
<img width="613" height="367" alt="image" src="https://github.com/user-attachments/assets/7aed61ab-6592-4228-b117-f9b2e4c9add9" />

~~~
#Bar Chart: 
height = [10, 24, 36, 40, 5] 
names = ['one', 'two', 'three', 'four', 'five'] 
c1=['red', 'green'] 
c2=['b', 'g'] 
plt.bar (names, height, width=0.8, color=c1) 
plt.xlabel('x - axis') 
plt.ylabel('y - axis') 
plt.title('My bar chart!') 
plt.show()
~~~
<img width="697" height="376" alt="image" src="https://github.com/user-attachments/assets/ea5268e1-ca7c-4906-b2cc-86621584d4f4" />

~~~
#Histogram: 
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x, bins = 10, color='blue', alpha=0.5) 
plt.show()
~~~
<img width="528" height="337" alt="image" src="https://github.com/user-attachments/assets/195729c4-b70c-49fa-8d50-5029f17c04cc" />


~~~
#Box Plot: 
np.random.seed(0) 
data=np.random.normal(loc=0, scale=1, size=100) 
data
~~~
<img width="622" height="310" alt="image" src="https://github.com/user-attachments/assets/7c4c5078-6db4-4185-bfb9-249f39661c53" />


~~~
fig, ax= plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values') 
ax.set_title('Box Plot')
~~~
<img width="705" height="415" alt="image" src="https://github.com/user-attachments/assets/f85423c4-7972-4881-9145-3ab487bdf075" />


# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.

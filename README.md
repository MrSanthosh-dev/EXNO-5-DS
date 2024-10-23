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
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```

![image](https://github.com/user-attachments/assets/766d423b-2dd3-4335-a713-9bba9d00ed29)

```
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph!')
plt.show()
```

![image](https://github.com/user-attachments/assets/1dc7c9e4-b990-4f77-bde9-570d3002c73c)

```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/4b58baa4-6c65-4ca9-8a1d-4ec78c7a0d05)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')

plt.show()
```

![image](https://github.com/user-attachments/assets/fa4af472-c4a1-4077-9c7c-7657f7914f4c)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![image](https://github.com/user-attachments/assets/3664b335-2684-406d-8413-00ebf2763db9)

```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
```
![image](https://github.com/user-attachments/assets/c371ae55-8717-40ce-b3ba-434b72a8e32b)


```
years=range(2000,2012)
apples= [0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```

![image](https://github.com/user-attachments/assets/4f6410bb-8a36-44a9-bfe2-42e93aaae51c)

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```

![image](https://github.com/user-attachments/assets/f3574f0e-ef83-4748-858e-8bde212e0fff)

```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```

![image](https://github.com/user-attachments/assets/11f7a1c5-abcf-4c05-be1b-914caa8e563d)

```
years=range(2000,2012)
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yeild of Oranges (tons per hectare)");
```

![image](https://github.com/user-attachments/assets/30153e5b-a06e-4f68-9ba5-e3b0fda465bb)

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```

![image](https://github.com/user-attachments/assets/ed9ede23-d8ac-457e-b28e-1bc37bebb658)

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
```

![image](https://github.com/user-attachments/assets/9ca6b375-5e5b-472c-aa70-a779761e8c43)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])

```
y
```

array([11, 12, 13, 14, 15, 16, 17, 18, 19, 20])


```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

![image](https://github.com/user-attachments/assets/24e7b2be-5a9e-4c5d-8949-9c2672e9f9eb)

```
y=x*x
y
```

array([ 0,  1,  4,  9, 16, 25, 36, 49, 64, 81])

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```

![image](https://github.com/user-attachments/assets/a0215ab6-b9bc-4814-abd2-97a40175d87f)

```
np.pi
```

3.141592653589793

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```


![image](https://github.com/user-attachments/assets/aff4a502-5a80-4ca2-9288-d53c703b6626)

```
import matplotlib.pyplot as plt
import numpy as np
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
plt.fill_between(x, y1 , color='red')
plt.fill_between(x, y2, color='yellow')
plt.plot(x, y1 , color='black')
plt.plot(x, y2, color='brown')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/d9fa4566-b7bd-43ce-9462-b7a071d0c0b5)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/user-attachments/assets/edd4bfe7-26d6-45b5-8a7f-0dfef6ef7aae)


```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,11]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/c0799505-04ce-43c4-a04d-1328bc0ecf49)


### Histogram

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No.of people')
plt.title('My histogram')
plt.show()
```


![image](https://github.com/user-attachments/assets/05b5b3d3-19f3-4932-a243-972dafeeed66)


### Boxplot

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```


![image](https://github.com/user-attachments/assets/082abd3c-004a-45b1-b649-8ebf87c665e6)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box plot')
```


![image](https://github.com/user-attachments/assets/bdd1b9f3-bde9-4c37-be92-513c343ff7cd)

### Pie chart

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,
autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```


![image](https://github.com/user-attachments/assets/b6fb842f-07f1-4417-9d82-a11d69a35298)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,
        startangle=90,shadow=True,explode=(0,0,0.1,0),
        radius=1.2,autopct='%1.1f%%')
plt.legend()
```


![image](https://github.com/user-attachments/assets/051a8839-8586-4c0b-9ca9-8c4b996c199a)



# Result:
  To Perform Data Visualization using matplot python library for the given datas is successful.
 

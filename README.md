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
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on same graph")
plt.legend()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/2fadf8b8-76aa-4943-a339-592ac5c96d7b)

```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth = 3, marker='o', markerfacecolor='blue', markersize=12)

plt.xlim(1,8)
plt.ylim(1,8)

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/27cb9a57-4194-402d-81e5-e154945222ef)

```
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='sienna', linewidth=3)
```

![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/ff22f12b-7fb1-4a3f-bcf7-8b5320a03c05)

```
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='chocolate', linewidth=3)
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/3ef6492e-cae2-45ac-b761-d84fbb241bcb)

```
years = range(2000, 2012) 
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ] 
 
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)'); 


plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel( 'Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/9c96022f-e099-4f27-aa56-7f4959a56f3b)

```
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)")
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/82b9bf6d-34c7-4f60-a08d-0e87d7570578)

```
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges'])
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/1e99da6b-a0b5-43ac-b34a-11390931d2cf)

```
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/db16ff6c-b075-4450-beb0-a719570ca6dc)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/baf67dc0-2328-4cd0-8956-1d2c78ee40c4)

```
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/0ca935ae-00c1-4961-bb6e-eb9345dcc61c)

```
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/289422e5-773b-4764-a34e-99f75b5bfb13)

```
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/cddec699-d792-4056-a687-02ce3363c490)

```
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/dfc80e06-a99a-47cd-9edf-71c9047de3e1)

```
import matplotlib.pyplot as plt
height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']
c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/bf465317-e2fc-4737-a96e-676f510dd8ab)

```
x = [2,8,10]
y = [11,16,9]
x2 = [3,9,11]
y2 = [6,15,7] 
plt.bar(x, y,color='chocolate')
plt.bar(x2, y2, color = 'darkgreen')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/955b028c-1aeb-4c7c-84e9-d1213c195f41)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10
plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)
plt.xlabel('age') 
plt.ylabel('No.Of.People')
plt.title('My Histogram')
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/be1cc969-ce83-49ea-ae3c-5269e8f4b6bc)

```
import matplotlib.pyplot as plt
import numpy as np 
np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/b07941dc-aa43-4b3f-8dd5-c993df27959e)

```
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('values')
ax.set_title('Box Plot')
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/51a9bedc-d285-4fe2-9434-7717ddfa0d47)

```
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/dbd6ff06-c11b-489a-8bb7-9caa745d7f4b)

```
activities = ['eat', 'sleep', 'work', 'play']
slices =[3,7,8,6]
colors=['r', 'y', 'g', 'b']
plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')
plt.legend()
```
![image](https://github.com/SanjithaBolisetti/EXNO-5-DS/assets/119393633/fb3b50a7-4384-4928-ba0c-d0247ddcdf4b)

# Result:
 Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.

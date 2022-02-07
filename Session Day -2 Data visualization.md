# Body mass Index 
**enter your weight
  enter your height


```python
#Body Mass index
#weight
#height
x=input("whats your weight")
y=input(" what is your height")
x=float(x)
y=float(y)
z=x/y**2
print(z)

```

    whats your weight45
     what is your height1.7
    15.570934256055365
    


```python
import numpy as np
import matplotlib.pyplot as plt
 
  
# creating the dataset
data = {'C':20, 'C++':15, 'Java':30,
        'Python':35}
courses = list(data.keys())
values = list(data.values())
  
fig = plt.figure(figsize = (10, 5))
 
# creating the bar plot
plt.bar(courses, values, color ='green',
        width = 0.4)
 
plt.xlabel("Courses offered")
plt.ylabel("No. of students enrolled")
plt.title("Students enrolled in different courses")
plt.show()
```


![png](output_2_0.png)



```python

```

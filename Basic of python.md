# basics of python


## operators


```python
print("hello worod")
```

    hello worod
    


```python
print(2+5)
```

    7
    


```python
print(9/5)
```

    1.8
    


```python
print(15%6)
```

    3
    


```python
x=5
```


```python
y=9
```


```python
print(x+y)
```

    14
    


```python
print(15//7)
```

    2
    


```python
m=3**3
```


```python
print(m)
```

    27
    

# PEMDAS 

## PRENTHISIS EXPONENT MULTIPLICATION DIVISION ADDITION SUBTRACTION



```python
print((9+2)*(3-2)/2*2**2)
```

    22.0
    

# Strings 


```python
print (' this is sting ')
```

     this is sting 
    


```python
print (" This is string ")
```

     This is string 
    


```python
print(    '''   this is sring    ''')
```

       this is sring    
    


```python
# print(" what's up   ?")
```

# commenting code
### use either # or use ctrl+/ to commets a specific area of code 



# Variable : are objects containing values 


```python
y= "I have a secrate sentance theek hai "
```


```python
print(y)
```

    I have a secrate sentance theek hai 
    


```python
x=5
```


```python
print(x)
```

    5
    


```python
type(y)
```




    str




```python
type(x)
```




    int




```python
print(type(y))
```

    <class 'str'>
    


```python
#print_type_class
```

# rules to assign variables 
### varialbe should contain letters  numbers and underscores 
###  should not start with numbers 
### space are not allowed 
### dont use keyword 
#### case sensitive (use lower case letters )




```python
fruit_basket= "mango","Orange"
print(type(fruit_basket))
```

    <class 'tuple'>
    

# using input function to enter values 


```python
fruit_basket=input("which is your favorate fruit?? ")
print(fruit_basket)
```


    ---------------------------------------------------------------------------

    KeyboardInterrupt                         Traceback (most recent call last)

    <ipython-input-26-7cdce04db790> in <module>
    ----> 1 fruit_basket=input("which is your favorate fruit?? ")
          2 print(fruit_basket)
    

    ~\anaconda3\1\lib\site-packages\ipykernel\kernelbase.py in raw_input(self, prompt)
        858                 "raw_input was called, but this frontend does not support input requests."
        859             )
    --> 860         return self._input_request(str(prompt),
        861             self._parent_ident,
        862             self._parent_header,
    

    ~\anaconda3\1\lib\site-packages\ipykernel\kernelbase.py in _input_request(self, prompt, ident, parent, password)
        902             except KeyboardInterrupt:
        903                 # re-raise KeyboardInterrupt, to truncate traceback
    --> 904                 raise KeyboardInterrupt("Interrupted by user") from None
        905             except Exception as e:
        906                 self.log.warning("Invalid Message:", exc_info=True)
    

    KeyboardInterrupt: Interrupted by user



```python
name = input("what is your name ")
greetings ="Hello"
print (greetings, name)
```


```python
name = input("your name")
age =input(" your age ")
print( "hello" ,name , " you are still young")
```

# Conditional operators


```python
#eqaul to ==
#not eqaul to !=
#less than <
#greater than >
#less than equal to <=
#greator than equal to >=

```


```python
print(4==4)
```


```python
print(4!=4)
```

# type conversition 


```python
age = input("Enter your age")
x=int(age)
if x>60:
    print(" you are senior citizion")
elif x<60:
    print(" you are not senior citizen")
elif 30<x>50:
    print(" Hello young lad")
else:
    print (" Hello boy")
```


```python
#implicit type conversion 
x=5
y=9.2
x=x*y
print(x)
print(type(x))
```


```python
# explicit type conversion
x= 150
y==14.63
x=int(y)
print(x)
print (type(x))
```

# Funtions 


```python
def Iqbal():
    x="Iqbal has many talents"
    print(x)
    print(x)
    print(x)
    
Iqbal()
    
```


```python
def iqbal(x):
    print(x)
    print(x)
    print(x)
    print(x)
    
iqbal("theek hai")
```


```python
def school_calculator(age,text):
    if age==5:
        print("Eesa can join school")
    elif age>5:
        print("Eesa can join higher school")
    else:
        print("Eesa is still a baby")
        
school_calculator(9,"Eesa")
```


```python
#future predicted age
def future_age(age):
    new_age=age+20
    return new_age
    print(new_age)

x=future_age(18)
print(x)
```

# for and while loop 


```python
x=0
while x<=5:
    print(x)
    x=x+1
    
```


```python
x=0
for x in range (0,20):
    print(x)
    x=x+1
```

# Arrays 


```python
days = ["Mon", "Tues","Wed","Thurs","Fri","Sat"]
for d in days :
    if (d=="Fri"):break #stop loop
#     if (d=="Fri"):continue 
       
print(d)
```

# Import libraries 


```python
import math
print(" the value of pie is ",math.pi)
```


```python
import statistics 
x=(12,10,156,49,32,89)
print("The mean value of x is ",statistics.mean(x))
```


# some important libraries of python are as below :
#### numpy pandas seabon matplotlib 

# Troubleshoting in python
*syntex error*
**semantic error**
**run time**




```python
#print(this is my house)  #syntex error
# print(25/0)             #runtime errorbb 

# name ="Iqbal ali"
# print (" Hello name ")  #semantic error
```





# indexing and data structure 


```python
a="samosa pakora"
a[0]
```


```python
a[3]
```


```python
len(a)
```


```python
a[0:6]
```


```python
a[-6]
```


```python
a[-7:-1]
```


```python
#operations on string :
food = "Biryani"
```


```python
#length of a string 
len(food)
```


```python
#capitalize word 
food.capitalize()
```


```python
#upper case 
food.upper()
```


```python
#lower case 
food.lower()
```


```python
#shriyani 
food.replace("B","sh")
```


```python
#character countb
food.count("i")
```

# Finding an index number ....


```python
name="This is my statement"
name
```


```python
name.find("e")
```


```python
food="I love samosa, raita, pakora and jalebi"
```


```python
food.split("a")
```


```python
food.split(",")
```

# Basic Data structure in python

# tuple / list / dictionary / set 

# tuple
**orderd collection of data
enclosed in round parenthesis
diffrent kind of elements can be stored 
elements cant be changed (un mutable)


```python
tup1=(1,"python",True,2.5)
tup1
```


```python
tup1[1]
```


```python
#last element is exclusive
tup1[0:3]
```


```python
len(tup1)
```


```python
tup2=(2,"iq",False,3.2)
tup2
```


```python
tup1+tup2
```


```python
tup1*2+tup2
```


```python
tup3 =(20,61,4.5,9,27)
tup3
```




    (20, 61, 4.5, 9, 27)




```python
max(tup3)
```




    61




```python
min(tup3)
```




    4.5




```python
tup3*2
```




    (20, 61, 4.5, 9, 27, 20, 61, 4.5, 9, 27)



# List
**. ordered collection of elements
. enclosed in [] sqare braketes
. mutable you can change the values 


```python
list1=[2,"python",3.5,False]
list1
```




    [2, 'python', 3.5, False]




```python
type(list1)
```




    list




```python
len(list1)
```




    4




```python
list1[2]
```




    3.5




```python
list2=[5,"r",885,2.9,True]
list2
```




    [5, 'r', 885, 2.9, True]




```python
list1+list2
```




    [2, 'python', 3.5, False, 5, 'r', 885, 2.9, True]




```python
list1*2
```




    [2, 'python', 3.5, False, 2, 'python', 3.5, False]




```python
list1.reverse()
list1
```




    [False, 3.5, 'python', 2]




```python
list1.append("theek hai")
list1
```




    [False, 3.5, 'python', 2, 'theek hai']




```python
list3=[20,100,50,90,10,5,6]
list3
```




    [20, 100, 50, 90, 10, 5, 6]




```python
list3.sort()
list3
```




    [5, 6, 10, 20, 50, 90, 100]



# Dictionaries 
**an un ordered collection of elements 
key and values 
curely braces used {}
mutable (changes the values)


```python
d1={"samosa":10,"jalebi":20,"Haleem":100, "biryani":150}
d1
```




    {'samosa': 10, 'jalebi': 20, 'Haleem': 100, 'biryani': 150}




```python
type(d1)
```




    dict




```python
food_keys=d1.keys()
food_keys
```




    dict_keys(['samosa', 'jalebi', 'Haleem', 'biryani'])




```python
food_values=d1.values()
food_values
```




    dict_values([10, 20, 100, 150])




```python
d1["samosa"]=50
d1
```




    {'samosa': 50, 'jalebi': 20, 'Haleem': 100, 'biryani': 150}




```python
d2={"chocolate":10,"maggie":20,"biscuites":100}
d2
```




    {'chocolate': 10, 'maggie': 20, 'biscuites': 100}




```python
d1.update(d2)
d1
```




    {'samosa': 50,
     'jalebi': 20,
     'Haleem': 100,
     'biryani': 150,
     'chocolate': 10,
     'maggie': 20,
     'biscuites': 100}



# set
**unordered and un indexed collection of elements 
curly braces {} used no duplicates are allowed 



```python
s1={2.5,"samosa",False,7}
s1.add("Saima")
s1
```




    {2.5, 7, False, 'Saima', 'samosa'}




```python
s1.pop()
s1
```




    {2.5, 7, 'Saima', 'samosa'}




```python
s1.remove("samosa")
s1
```




    {2.5, 7, 'Saima'}




```python
s1.discard
```


```python
A = {'a', 'b', 'c', 'd'}
B = {'c', 'f', 'g'}

# Equivalent to A-B
print(A.difference(B))

# Equivalent to B-A
print(B.difference(A))
```

    {'b', 'a', 'd'}
    {'f', 'g'}
    


```python
numbers = {1, 2, 3, 4}
new_numbers = numbers.copy()

new_numbers.add(5)

print('numbers: ', numbers)
print('new_numbers: ', new_numbers)
```

    numbers:  {1, 2, 3, 4}
    new_numbers:  {1, 2, 3, 4, 5}
    


```python
numbers = {2, 3, 4, 5}

numbers.discard(3)
print('numbers = ', numbers)

numbers.discard(10)
print('numbers = ', numbers)
```

    numbers =  {2, 4, 5}
    numbers =  {2, 4, 5}
    


```python
A = {2, 3, 5}
B = {1, 3, 5}

# compute intersection between A and B
print(A.intersection(B))


```

    {3, 5}
    


```python
A = {100, 7, 8}
B = {200, 4, 5}
C = {300, 2, 3}
D = {100, 200, 300}

print(A.intersection(D))
print(B.intersection(D))
print(C.intersection(D))
print(A.intersection(B, C, D))

```

    {100}
    {200}
    {300}
    set()
    


```python
A = {100, 7, 8}
B = {200, 4, 5}
C = {300, 2, 3, 7}
D = {100, 200, 300}

print(A & C)
print(A & D)

print(A & C & D)

print(A & B & C & D)
```

    {7}
    {100}
    set()
    set()
    


```python
A ={'a', 'b', 'c', 'd'}

print('Return Value is', A.pop())
print('A = ', A)
```

    Return Value is b
    A =  {'a', 'c', 'd'}
    


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


```python

```

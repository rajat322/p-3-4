# Question 31

### **Question:**

>***Define a function which can print a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys.***

----------------------

### Hints: 
```
Use dict[key]=value pattern to put entry into a dictionary.Use ** operator to get power of a number.Use range() for loops.
```

def printDict():
    dict={i:i**2 for i in range(1,21)}   
    print(dict)

printDict()


# Question 32

### **Question:**

>***Define a function which can generate a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys. The function should just print the keys only.***

----------------------

### Hints:
``` 
Use dict[key]=value pattern to put entry into a dictionary.Use ** operator to get power of a number.Use range() for loops.Use keys() to iterate keys in the dictionary. Also we can use item() to get key/value pairs.
```def printDict():
    dict = {i: i**2 for i in range(1, 21)}
    print(dict.keys())      # print keys of a dictionary

printDict()


# Question 33

### **Question:**

>***Define a function which can generate and print a list where the values are square of numbers between 1 and 20 (both included).***

----------------------

### Hints:
```
Use ** operator to get power of a number.Use range() for loops.Use list.append() to add values into a list.
```

def printList():
    lst = [i ** 2 for i in range(1, 21)]
    print(lst)

printList()

# Question 34

### **Question:**

>***Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the first 5 elements in the list.***

----------------------

### Hints:
```
Use ** operator to get power of a number.Use range() for loops.Use list.append() to add values into a list.Use [n1:n2] to slice a list
```

def printList():
    lst = [i ** 2 for i in range(1, 21)]

    for i in range(5):
        print(lst[i])

printList()

# Question 35

### **Question:**

>***Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the last 5 elements in the list.***

----------------------
### Hints:
```
Use ** operator to get power of a number.Use range() for loops.Use list.append() to add values into a list.Use [n1:n2] to slice a list
```



def printList():
    lst = [i ** 2 for i in range(1, 21)]
    for i in range(19,14,-1):
        print(lst[i])

printList()
# Question 36

### **Question:**

>***Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print all values except the first 5 elements in the list.***

----------------------
```
Hints: Use ** operator to get power of a number.Use range() for loops.Use list.append() to add values into a list.Use [n1:n2] to slice a list
```
def printList():
    lst = [i ** 2 for i in range(1, 21)]
    for i in range(5,20):
        print(lst[i])

printList()

# Question 37

### **Question:**

>***Define a function which can generate and print a tuple where the value are square of numbers between 1 and 20 (both included).***


----------------------

### Hints: 
```
Use ** operator to get power of a number.Use range() for loops.Use list.append() to add values into a list.Use tuple() to get a tuple from a list.
```

def printTupple():
    lst = [i ** 2 for i in range(1, 21)]
    print(tuple(lst))

printTupple()



### Comment
***Problems of this section is very much easy and all of those are of a modification of same type problem which mainly focused on using some commonly used function works with list,dictionary, tupple.In my entire solutions, I havn't tried to solve problems in efficient way.Rather I tried to solve in a different way that I can.This will help a beginner to know how simplest problems can be solved in different ways.*** 




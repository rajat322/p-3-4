# Question 38

### **Question:**

>***With a given tuple (1,2,3,4,5,6,7,8,9,10), write a program to print the first half values in one line and the last half values in one line.***

----------------------

### Hints:
>***Use [n1:n2] notation to get a slice from a tuple.***




def printTupple():
    lst = [i ** 2 for i in range(1, 21)]
    print(tuple(lst))

printTupple()

# Question 39

### **Question:**

>***Write a program to generate and print another tuple whose values are even numbers in the given tuple (1,2,3,4,5,6,7,8,9,10).***

----------------------

### Hints:
>***Use "for" to iterate the tuple. Use tuple() to generate a tuple from a list.***



tpl = (1,2,3,4,5,6,7,8,9,10)
tpl1 = tuple(i for i in tpl if i%2 == 0)
print(tpl1)


# Question 40

### **Question:**

>***Write a program which accepts a string as input to print "Yes" if the string is "yes" or "YES" or "Yes", otherwise print "No".***







### Hints: 
>***Use if statement to judge condition.***





# Question 41

### **Question:**

>***Write a program which can map() to make a list whose elements are square of elements in [1,2,3,4,5,6,7,8,9,10].***

----------------------

### Hints: 
>***Use map() to generate a list.Use lambda to define anonymous functions.***

li = [1,2,3,4,5,6,7,8,9,10]
squaredNumbers = map(lambda x: x**2, li) 
print(list(squaredNumbers))   


# Question 42

### **Question:**

>***Write a program which can map() and filter() to make a list whose elements are square of even number in [1,2,3,4,5,6,7,8,9,10].***

----------------------
### Hints: 
>***Use map() to generate a list.Use filter() to filter elements of a list.Use lambda to define anonymous functions.***


def even(x):
    return x%2==0

def squer(x):
    return x*x

li = [1,2,3,4,5,6,7,8,9,10]
li = map(squer,filter(even,li))  
print(list(li))




# Question 43

### **Question:**

>***Write a program which can filter() to make a list whose elements are even number between 1 and 20 (both included).***

----------------------
### Hints: 
>***Use filter() to filter elements of a list.Use lambda to define anonymous functions.***



def even(x):
    return x%2==0

evenNumbers = filter(even, range(1,21))
print(list(evenNumbers))



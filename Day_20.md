
# Question 80

### **Question**

>***Please write a program to print the list after removing even numbers in [5,6,77,45,22,12,24].***


----------------------
### Hints 
> ***Use list comprehension to delete a bunch of element from a list.***

def isEven(n):
    return n%2!=0

li = [5,6,77,45,22,12,24]
lst = list(filter(isEven,li))
print(lst)


# Question 81

### **Question**

>***By using list comprehension, please write a program to print the list after removing numbers which are divisible by 5 and 7 in [12,24,35,70,88,120,155].***

----------------------
### Hints 
> ***Use list comprehension to delete a bunch of element from a list.***

li = [12,24,35,70,88,120,155]
li = [x for x in li if x % 35!=0]
print(li)

# Question 82

### **Question**

>***By using list comprehension, please write a program to print the list after removing the 0th, 2nd, 4th,6th numbers in [12,24,35,70,88,120,155].***


### Hints 
>***Use list comprehension to delete a bunch of element from a list.
Use enumerate() to get (index, value) tuple.***

li = [12,24,35,70,88,120,155]
li = [li[i] for i in range(len(li)) if i%2 != 0]
print(li)


# Question 83

### **Question**

>***By using list comprehension, please write a program to print the list after removing the 2nd - 4th numbers in [12,24,35,70,88,120,155].***

----------------------
### Hints 
> ***Use list comprehension to delete a bunch of element from a list.
Use enumerate() to get (index, value) tuple.***



li = [12,24,35,70,88,120,155]
li = [li[i] for i in range(len(li)) if i<3 or 4<i]
print(li)



# Question 84

### **Question**

> ***By using list comprehension, please write a program generate a 3\*5\*8 3D array whose each element is 0.***


----------------------
### Hints 
> ***Use list comprehension to make an array.***

array = [[ [0 for col in range(8)] for col in range(5)] for row in range(3)]
print array
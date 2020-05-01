
# Question 85

### **Question**

>***By using list comprehension, please write a program to print the list after removing the 0th,4th,5th numbers in [12,24,35,70,88,120,155].***


----------------------
### Hints 
> ***Use list comprehension to delete a bunch of element from a list.Use enumerate() to get (index, value) tuple.***

li = [12,24,35,70,88,120,155]
li = [li[i] for i in range(len(li)) if i not in (0,4,5)]
print(li)


# Question 86

### **Question**

>***By using list comprehension, please write a program to print the list after removing the value 24 in [12,24,35,24,88,120,155].***

----------------------
### Hints 
> ***Use list's remove method to delete a value.***

li = [12,24,35,24,88,120,155]
li.remove(24)  
print(li)



# Question 87

### **Question**

>***With two given lists [1,3,6,78,35,55] and [12,24,35,24,88,120,155], write a program to make a list whose elements are intersection of the above given lists.***

----------------------
### Hints 
>***Use set() and "&=" to do set intersection operation.***


list1 = [1,3,6,78,35,55]
list2 = [12,24,35,24,88,120,155]
set1= set(list1)
set2= set(list2)
intersection = set1 & set2
print(intersection)
```

# Question 88

### **Question**

>***With a given list [12,24,35,24,88,120,155,88,120,155], write a program to print this list after removing all duplicate values with original order reserved.***

----------------------
### Hints 
> ***Use set() to store a number of values without duplicate.***

li = [12,24,35,24,88,120,155,88,120,155]
for i in li:
    if li.count(i) > 1:
        li.remove(i)
print(li)


# Question 89

### **Question**

>***Define a class Person and its two child classes: Male and Female. All classes have a method "getGender" which can print "Male" for Male class and "Female" for Female class.***


----------------------
### Hints 
> ***Use Subclass(Parentclass) to define a child class.***


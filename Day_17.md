
# Question 65

### **Question**

>***Please write assert statements to verify that every number in the list [2,4,6,8] is even.***


----------------------
### Hints
> ***Use "assert expression" to make assertion.***


data = [2,4,5,6]
for i in data:
    assert i%2 == 0, "{} is not an even number".format(i)

# Question 66

### **Question**

>***Please write a program which accepts basic mathematic expression from console and print the evaluation result.***

>***Example:
If the following n is given as input to the program:***
```
35 + 3
```
>***Then, the output of the program should be:***
```
38
```

### Hints
> ***Use eval() to evaluate an expression.***


expression = input()
ans = eval(expression)
print(ans)



# Question 67

### **Question**

>***Please write a binary search function which searches an item in a sorted list. The function should return the index of element to be searched in the list.***

----------------------
### Hints
>***Use if/elif to deal with conditions.***




# Question 68

### **Question**

>***Please generate a random float where the value is between 10 and 100 using Python module.***

----------------------
### Hints
> ***Use random.random() to generate a random float in [0,1].***

import random
rand_num = random.uniform(10,100)
print(rand_num)

# Question 69

### **Question**

>***Please generate a random float where the value is between 5 and 95 using Python module.***


----------------------
### Hints
> ***Use random.random() to generate a random float in [0,1].***



import random
rand_num = random.uniform(5,95)
print(rand_num)

# Question 26

### **Question:**

>***Define a function which can compute the sum of two numbers.***

----------------------

### Hints:
>***Define a function with two numbers as arguments. You can compute the sum in the function and return the value.***

sum = lambda n1,n2 : n1 + n2      
print(sum(1,2))


# Question 27

### **Question:**

>***Define a function that can convert a integer into a string and print it in console.***

----------------------
### Hints: 
>***Use str() to convert a number to string.***


conv = lambda x : str(x)
n = conv(10)
print(n)
print(type(n))   


# Question 28

### **Question:**

>***Define a function that can receive two integer numbers in string form and compute their sum and then print it in console.***

----------------------
### Hints: 
>***Use int() to convert a string to integer.***

sum = lambda s1,s2 : int(s1) + int(s2)
print(sum("10","45")) 

# Question 29

### **Question:**

>***Define a function that can accept two strings as input and concatenate them and then print it in console.***

----------------------

### Hints: 
>***Use + sign to concatenate the strings.***


sum = lambda s1,s2 : s1 + s2
print(sum("10","45"))  

# Question 30

### **Question:**

>***Define a function that can accept two strings as input and print the string with maximum length in console. If two strings have the same length, then the function should print all strings line by line.***

----------------------
### Hints: 
>***Use len() function to get the length of a string.***


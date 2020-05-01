
# Question 90

### **Question**

>***Please write a program which count and print the numbers of each character in a string input by console.***

>***Example:
If the following string is given as input to the program:***
```
abcdefgabc
```
>***Then, the output of the program should be:***
```
a,2
c,2
b,2
e,1
d,1
g,1
f,1
```
### Hints 
> ***Use dict to store key/value pairs.
Use dict.get() method to lookup a key with default value.***

import string

s = input()
for letter in string.ascii_lowercase:
    cnt = s.count(letter)
    if cnt > 0:
        print("{},{}".format(letter,cnt))


# Question 91

### **Question**

>***Please write a program which accepts a string from console and print it in reverse order.***

>**Example:
If the following string is given as input to the program:***
```
rise to vote sir
```
>***Then, the output of the program should be:***
```
ris etov ot esir
```
### Hints 
> ***Use list[::-1] to iterate a list in a reverse order.***

s = input()
s = ''.join(reversed(s))
print(s)

# Question 92

### **Question**

>***Please write a program which accepts a string from console and print the characters that have even indexes.***

>***Example:
If the following string is given as input to the program:***
```
H1e2l3l4o5w6o7r8l9d
```
>***Then, the output of the program should be:***
```
Helloworld
```
### Hints 
>***Use list[::2] to iterate a list by step 2.***

s = "H1e2l3l4o5w6o7r8l9d"
s = [ s[i] for i in range(len(s)) if i%2 ==0 ]
print(''.join(s))

# Question 93

### **Question**

>***Please write a program which prints all permutations of [1,2,3]***

----------------------
### Hints 
> ***Use itertools.permutations() to get permutations of list.***

import itertools
print list(itertools.permutations([1,2,3]))

# Question 94

### **Question**

>***Write a program to solve a classic ancient Chinese puzzle: 
We count 35 heads and 94 legs among the chickens and rabbits in a farm. How many rabbits and how many chickens do we have?***


----------------------
### Hints 
> ***Use for loop to iterate all possible solutions.***



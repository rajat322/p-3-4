# Question 10

### **Question**

>***Write a program that accepts a sequence of whitespace separated words as input and prints the words after removing all duplicate words and sorting them alphanumerically.***

>***Suppose the following input is supplied to the program:***
```
hello world and practice makes perfect and hello world again
```
>***Then, the output should be:***
```
again and hello makes perfect practice world
```

word = sorted(list(set(input().split())))             
                                         
print(" ".join(word))

### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.We use set container to remove duplicated data automatically and then use sorted() to sort the data.***

-------------------

---------------------------

# Question 11

### **Question**

>***Write a program which accepts a sequence of comma separated 4 digit binary numbers as its input and then check whether they are divisible by 5 or not. The numbers that are divisible by 5 are to be printed in a comma separated sequence.***

>***Example:***
```
0100,0011,1010,1001
```
>***Then the output should be:***
```
1010
```
>***Notes: Assume the data is input by console.***

----------------------

### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***



data = input().split(',')
data = list(filter(lambda i:int(i,2)%5==0,data))    
print(",".join(data))

# Question 12

### **Question:**

>***Write a program, which will find all such numbers between 1000 and 3000 (both included) such that each digit of the number is an even number.The numbers obtained should be printed in a comma-separated sequence on a single line.***

----------------------

### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

def check(element):
    return all(ord(i)%2 == 0 for i in element)  

lst = [str(i) for i in range(1000,3001)]        
lst = list(filter(check,lst))                   
print(",".join(lst))

# Question 13

### **Question:**

>***Write a program that accepts a sentence and calculate the number of letters and digits.***

>***Suppose the following input is supplied to the program:***

```
hello world! 123
```

>***Then, the output should be:***
```
LETTERS 10
DIGITS 3
```
----------------------

### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***


word = input()
letter,digit = 0,0

for i in word:
    if ('a'<=i and i<='z') or ('A'<=i and i<='Z'):
        letter+=1
    if '0'<=i and i<='9':
        digit+=1

print("LETTERS {0}\nDIGITS {1}".format(letter,digit))





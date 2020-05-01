

# Question 60

### **Question**

>***Write a program to compute:***
```
f(n)=f(n-1)+100 when n>0
and f(0)=0
```
>***with a given n input by console (n>0).***

>***Example:
If the following n is given as input to the program:***
```
5
```
>***Then, the output of the program should be:***
```
500
```
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
> ***We can define recursive function in Python.***



def f(n):
    if n == 0:
        return 0
    return f(n-1) + 100

n = int(input())
print(f(n))


# Question 61

### **Question**

>***The Fibonacci Sequence is computed based on the following formula:***
```
f(n)=0 if n=0
f(n)=1 if n=1
f(n)=f(n-1)+f(n-2) if n>1
```
>***Please write a program to compute the value of f(n) with a given n input by console.***

>***Example:
If the following n is given as input to the program:***
```
7
```
>***Then, the output of the program should be:***
```
13
```
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
> ***We can define recursive function in Python.***



def f(n):
    if n < 2:
        return n
    return f(n-1) + f(n-2)

n = int(input())
print(f(n))


# Question 62

### **Question**

>***The Fibonacci Sequence is computed based on the following formula:***
```
f(n)=0 if n=0
f(n)=1 if n=1
f(n)=f(n-1)+f(n-2) if n>1
```
>***Please write a program to compute the value of f(n) with a given n input by console.***

>***Example:
If the following n is given as input to the program:***
```
7
```
>***Then, the output of the program should be:***
```
0,1,1,2,3,5,8,13
```
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
>***We can define recursive function in Python.
Use list comprehension to generate a list from an existing list.
Use string.join() to join a list of strings.***






# Question 63

### **Question**

>***Please write a program using generator to print the even numbers between 0 and n in comma separated form while n is input by console.***

>***Example:
If the following n is given as input to the program:***
```
10
```
>***Then, the output of the program should be:***
```
0,2,4,6,8,10
```
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
> ***Use yield to produce the next value in generator.***


n = int(input())

for i in range(0, n+1, 2):
  if i < n - 1:
    print(i, end = ',' )
  else:
    print(i)




# Question 64

### **Question**

>***Please write a program using generator to print the numbers which can be divisible by 5 and 7 between 0 and n in comma separated form while n is input by console.***

>***Example:
If the following n is given as input to the program:***
```
100
```
>***Then, the output of the program should be:***
```
0,35,70
```
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
> ***Use yield to produce the next value in generator.***

def generate(n):
    for i in range(n+1):
        if i % 35 == 0:    # 5*7 = 35, if a number is divisible by a & b then it is also divisible by a*b
            yield i

n = int(input())
resp = [str(i) for i in generate(n)]
print(",".join(resp))


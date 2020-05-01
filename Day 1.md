
# Question 1

### **Question:**

> ***Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5,
between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line.***

--------------------------------------
### Hints: 
> ***Consider use range(#begin, #end) method.***
l=[]
for i in range(2000, 3201):
    if (i%7==0) and (i%5!=0):
        l.append(str(i))

print (','.join(l))



# Question 2

### **Question:**

> ***Write a program which can compute the factorial of a given numbers.The results should be printed in a comma-separated sequence on a single line.Suppose the following input is supplied to the program: 8
Then, the output should be:40320***

--------------------
### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***
 n = int(input())
    def shortFact(x): return 1 if x <= 1 else x*shortFact(x-1)
   
   print(shortFact(n))

 
 

# Question 3

### **Question:**

>***With a given integral number n, write a program to generate a dictionary that contains (i, i x i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary.Suppose the following input is supplied to the program: 8***

>***Then, the output should be:***
```
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}

n = int(input())
ans = {}
for i in range (1,n+1):
    ans[i] = i * i
print(ans)

### Hints: 
>***In case of input data being supplied to the question, it should be assumed to be a console input.Consider use dict()***

-----------------


----------------------------------

## Conclusion
***These was the solved problems of day 1. The above problems are very easy for the basic syntex learners.I have shown some easy ways of coding in my solutions. Lets see how to face and attack new problems in the next day.***





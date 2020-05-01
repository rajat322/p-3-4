
# Question 14

### **Question:**

>***Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters.***

>***Suppose the following input is supplied to the program:***
```
Hello world!
```
>***Then, the output should be:***
```
UPPER CASE 1
LOWER CASE 9
```
word = input()
upper,lower = 0,0

for i in word:
    if 'a'<=i and i<='z' :
        lower+=1
    if 'A'<=i and i<='Z':
        upper+=1

print("UPPER CASE {0}\nLOWER CASE {1}".format(upper,lower))

### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***

-------------------


----------------------
# Question 15

### **Question:**

>***Write a program that computes the value of a+aa+aaa+aaaa with a given digit as the value of a.***

>***Suppose the following input is supplied to the program:***

```
9
```

>***Then, the output should be:***
```
11106
```
---------------------
### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.***
a = input()
total = int(a) + int(2*a) + int(3*a) + int(4*a)  # N*a=Na, for example  a="23", 2*a="2323",3*a="232323"
print(total)
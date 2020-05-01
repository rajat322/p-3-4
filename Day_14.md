
# Question 51

### **Question**

> ***Write a function to compute 5/0 and use try/except to catch the exceptions.***

----------------------
### Hints 
> ***Use try/except to catch exceptions.***

def divide():
    return 5/0

try:
    divide()
except ZeroDivisionError as ze:
    print("Why on earth you are dividing a number by ZERO!!")
except:
    print("Any other exception")


# Question 52

### **Question**

> ***Define a custom exception class which takes a string message as attribute.***

----------------------
### Hints 
> ***To define a custom exception, we need to define a class inherited from Exception.***




# Question 53

### **Question**

> ***Assuming that we have some email addresses in the "username@companyname.com" format, please write program to print the user name of a given email address. Both user names and company names are composed of letters only.***

> ***Example:
If the following email address is given as input to the 
program:***
```
john@google.com
```
> ***Then, the output of the program should be:***
```
john
```
> ***In case of input data being supplied to the question, it should be assumed to be a console input.***

----------------------
### Hints 
> ***Use \w to match letters.***

email = "john@google.com"
email = email.split('@')
print(email[0])


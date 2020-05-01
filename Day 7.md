# Question 20

### **Question:**

>***Define a class with a generator which can iterate the numbers, which are divisible by 7, between a given range 0 and n.***

----------------------

### Hints:
>***Consider use class, function and comprehension.***

class Divisible:
    
    def by_seven(self, n):
        for number in range(n + 1):
            if number % 7 == 0: yield number


divisible = Divisible()
generator = divisible.by_seven(int(input("Please insert a number. --> ")))
for number in generator:
    print(number)



# Question 21

### **Question:**

>***A robot moves in a plane starting from the original point (0,0). The robot can move toward UP, DOWN, LEFT and RIGHT with a given steps. The trace of robot movement is shown as the following:***
```
UP 5
DOWN 3
LEFT 3
RIGHT 2
```
>***The numbers after the direction are steps. Please write a program to compute the distance from current position after a sequence of movement and original point. If the distance is a float, then just print the nearest integer.***
***Example:***
***If the following tuples are given as input to the program:***
```
UP 5
DOWN 3
LEFT 3
RIGHT 2
```
>***Then, the output of the program should be:***
```
2
```

----------------------
### Hints:
>***In case of input data being supplied to the question, it should be assumed to be a console input.Here distance indicates to euclidean distance.Import math module to use sqrt function.***


import  math

x,y = 0,0
while True:
    s = input().split()
    if not s:
        break
    if s[0]=='UP':                 
        x-=int(s[1])             
    if s[0]=='DOWN':
        x+=int(s[1])
    if s[0]=='LEFT':
        y-=int(s[1])
    if s[0]=='RIGHT':
        y+=int(s[1])
                                    
dist = round(math.sqrt(x**2 + y**2))  
print(dist)


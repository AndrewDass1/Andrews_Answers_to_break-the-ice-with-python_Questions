# Day 1 Solutions

# Question 1

# Q1 Task
Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line. <br>

# Q1 Procedure
1. Create a for loop to loop through numbers between and including 2000 and 3200:
```
for i in range(2000, 3201):
```

2. Within the for loop, include an if statement to print the numbers within the range 2000 to 3200 that are divisible by 7 and also **not** divisible by 5:
```
if i % 7 == 0 and i % 5 !=0 :
```

3. Use the 'end = " "' to print every output on the same line:
```
print(i, end=" ")
```

# Q1 Solution
```
for i in range(2000, 3201):
  if i % 7 == 0 and i % 5 !=0 :
    print(i, end=" ")
``` 
   
# Question 2

# Q2 Task
Write a program which can compute the factorial of a given numbers.The results should be printed in a comma-separated sequence on a single line.Suppose the following input is supplied to the program: 8 Then, the output should be:40320 <br>

# Q2 Procedure
1. Declare and name a variable to take in an integer data type:
```
num = int(input(""))
```
2. Initiate another variable to be equal to 1:
```
product_of_num = 1
```
The variable "product_of_num = 1" value can be placed within a for loop or while loop for its value to constantly be updated by the variable 'num' input to calculate the factorial. <br>
<br>
3. If the 'num' variable was given a number equal to or less than 0, include a while statement to reask to give an input greater than 0 for the variable 'num': 
```
while num <= 0:
  num = int(input(""))
```
4.  Declare either a for loop or while loop to calculate the factorial and print the end result:
```
while (num > 0): 
  product_of_num = product_of_num * num 
  num -= 1 

print(product_of_num)
```

# Q2 Solution
```
num = int(input(""))
product_of_num = 1

while num <= 0:
  num = int(input(""))

while (num > 0): 
  product_of_num = product_of_num * num 
  num -= 1 

print(product_of_num)
```

# Question 3
```
dictionary_of_num = {} 
num = int(input("")) 
num2 = 1

for i in range(1, num+1): 
  dictionary_of_num[num2] = num2**num2 
  num2+=1 

print(dictionary_of_num) 
```

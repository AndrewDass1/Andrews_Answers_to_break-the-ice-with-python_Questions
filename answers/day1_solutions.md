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

# Q3 Task
With a given integral number n, write a program to generate a dictionary that contains (i, i x i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary.Suppose the following input is supplied to the program: 8 <br>
<br>
Then, the output should be:
```
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
```

# Q3 Procedure
1. Create a variable that holds an empty dictionary:
```
dictionary_of_num = {} 
```
2. Create another variable that takes an integer input:
```
num = int(input("")) 
```
3. Use a for loop to have the dictionaries indexes update with the the square of the number 1 to the number that was previously inputed as 'num' for the ending range. <br>
<br>  

Another variable 'num2' was declared to equal 1 and it is updated within the for loop to calcuate the square of its index position value:
```
num2 = 1

for i in range(1, num+1): 
  dictionary_of_num[num2] = num2**num2 
  num2+=1 

print(dictionary_of_num) 
```

In the line of code 'for in range(1, num+1)', it is written as 'num+1' since the range() function takes two parameters from a number to start from and to end at. The number it ends at is always the number -1 from the number specified. If the user asked num = 8, then the range function would print the numbers 1,2,3,4,5,6,7 and not 8. To fix this, num+1 was inserted within the range() ending parameter to print 8.  

# Q3 Demonstration
If num was inputted to take the integer = 8, then the dictionary would calcuate the following shown below: <br>
<br>
When num2 = 1, then the dictionary will calculate: <br>
<br>
dictionary_of_num[1] = 1 * 1 <br>

<br>
When num2 = 2, then the dictionary will calculate: <br>
<br>
dictionary_of_num[2] = 2 * 2 <br>
<br>

<br>
When num2 = 3, then the dictionary will calculate: <br>
<br>
dictionary_of_num[3] = 3 * 3 <br>
<br>

<br>
When num2 = 4, then the dictionary will calculate: <br>
<br>
dictionary_of_num[4] = 4 * 4 <br>
<br>

<br>
When num2 = 5, then the dictionary will calculate: <br>
<br>
dictionary_of_num[5] = 5 * 5 <br>
<br>

<br>
When num2 = 6, then the dictionary will calculate: <br>
<br>
dictionary_of_num[6] = 6 * 6 <br>
<br>

<br>
When num2 = 7, then the dictionary will calculate: <br>
<br>
dictionary_of_num[7] = 7 * 7 <br>
<br>

<br>
When num2 = 8, then the dictionary will calculate: <br>
<br>
dictionary_of_num[8] = 8 * 8 <br>
<br>

When printing the variable that contains the dictionary with the command
```
print(dictionary_of_num)
```
The following will show all the index numbers with the square value of the index:
```
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
```

# Q3 Solution
```
dictionary_of_num = {} 
num = int(input("")) 
num2 = 1

for i in range(1, num+1): 
  dictionary_of_num[num2] = num2**num2 
  num2+=1 

print(dictionary_of_num) 
```

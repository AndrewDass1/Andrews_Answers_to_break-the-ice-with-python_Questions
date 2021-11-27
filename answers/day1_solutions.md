# Day 1 Solutions

# Question 1

# Task
Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line. <br>

# Procedure
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

# Solution
```
for i in range(2000, 3201):
  if i % 7 == 0 and i % 5 !=0 :
    print(i, end=" ")
``` 
   
# Question 2
```
num = int(input(""))
product_of_num = 1

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

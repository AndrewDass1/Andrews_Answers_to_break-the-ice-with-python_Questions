# Day 2 Solutions

# Question 4

# Q4 Task
Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple which contains every number.Suppose the following input is supplied to the program:

# Q4 Procedure
1. Declare a variable to take an integer data type:
```
num = int(input("")) 
```
2. Declare another variable that is an empty list:
```
list_of_num = []
```
3. Create a for loop to add integers of your choice to the empty list variable with the append command:
```
for i in range(0, num): 
  enter_num = int(input("")) 
  list_of_num.append(enter_num) 
```
4. Create another variable to cast the list to a tuple:
```
num_tuple = tuple(list_of_num)
```
5. Print out the list and tuple variables:
```
print(list_of_num)
print(num_tuple) 
```
# Q4 Solution
```
num = int(input("")) 
list_of_num = []

for i in range(0, num): 
  enter_num = int(input("")) 
  list_of_num.append(enter_num) 

num_tuple = tuple(list_of_num)

print(list_of_num)
print(num_tuple) 
```

# Question 5

# Question 6

# Q6 Task
Write a program that calculates and prints the value according to the given formula: <br>
<br>
Q = Square root of [(2 _ C _ D)/H] <br>
<br>
Following are the fixed values of C and H: <br>
<br>
C is 50. H is 30. <br>
<br>
D is the variable whose values should be input to your program in a comma-separated sequence.For example Let us assume the following comma separated input sequence is given to the program:

# Q6 Procedure
1. Declare variables C, D, and H:
```
C = 50 
D = int(input("")) 
H = 30
```
2. Declare Q to perform the formula asked:
```
Q = ((2* C *D) / H) ** (1/2) 
```
3. Print out variable Q:  
```
print(Q) 
```

# Q6 Solution
```
C = 50 
D = int(input("")) 
H = 30

Q = ((2* C *D) / H) ** (1/2) 
print(Q) 
```

With a Function:
```
def math_formula():

  C = 50 
  D = int(input("")) 
  H = 30 

  Q = ((2 * C * D) / H) ** (1/2)
  return(Q) 

math_formula()
```

# Question 7


# Question 8

# Q8 Task
Write a program that accepts a comma separated sequence of words as input and prints the words in a comma-separated sequence after sorting them alphabetically. <br>
<br>
Suppose the following input is supplied to the program:
```
without,hello,bag,world
```
Then, the output should be:
```
bag,hello,without,world
```


# Q8 Procedure
1. Declare a variable to input a sequence of words: 
```
statement = input("").split(",")
```

2. Declare another variable to sort the statement
```
sorted_statement = sorted(statement)
```

3. Declare a for loop to print out the variables with the sorted sequences by using another variable that is declared to be a counter and to be updated within the for loop:
```
num_counter = 0

for i in range(0, len(statement)):
  print(sorted_statement[num_counter], end=" ")
  num_counter += 1 
```

# Q8 Solution
```
statement = input("").split(",")
num_counter = 0
sorted_statement = sorted(statement)

#Split shows if the statement is separated by , then it will be sorted

for i in range(0, len(statement)):
  print(sorted_statement[num_counter], end=" ")
  num_counter += 1 
```
  
# Question 9

# Q9 Task
Write a program that accepts sequence of lines as input and prints the lines after making all characters in the sentence capitalized. <br>
<br>
Suppose the following input is supplied to the program:
```
Hello world
Practice makes perfect
```
Then, the output should be:
```
HELLO WORLD
PRACTICE MAKES PERFECT
```
# Q9 Procedure
1. Declare a number to take an integer data type:
```
num_of_statements = int(input(""))
```
2. Declare a variable to be an empty list:
```
statementlist = []
```
3. Declare a for loop to input words in the empty list:
```
for i in range(0, num_of_statements):
  statement = input("").upper()
  statementlist.append(statement)
```
4. Use another for loop and optionally a variable to print out the terms in the for loop:
```
num_counter = 0

for i2 in range(0, num_of_statements):
  print(statementlist[num_counter])
  num_counter += 1
```

# Q9 Solution
```
num_of_statements = int(input(""))
statementlist = []
num_counter = 0

for i in range(0, num_of_statements):
  statement = input("").upper()
  statementlist.append(statement)

for i2 in range(0, num_of_statements):
  print(statementlist[num_counter])
  num_counter += 1
```

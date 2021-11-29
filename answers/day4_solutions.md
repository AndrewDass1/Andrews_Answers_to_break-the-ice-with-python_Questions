# Day 4 Solutions

# Question 14

# Q4 Task
Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters. <br>
<br>
Suppose the following input is supplied to the program: 
```
Hello world!
```
Then, the output should be:
```
UPPER CASE 1
LOWER CASE 9
```

# Q4 Procedure
1. Declare a variable to take a string
   Below, a function was used with a predefined variable to be used as a string:
```
def lowerUpperCase(statement): 
```
2. Declare a for loop and if and else statements to cycle through the string data type indexes. Declare other variables neccessary to peform this task. For this demonstration, the following variables were created:
```
index_counter = 0 
uppercase_counter = 0 
lowercase_counter = 0 
case_counter_list = [] 
```
index_counter goes through the index of the string to see whether it is an uppercase or lowercase letter. <br>
uppercase_counter keeps track of how many capital letters there are in a word. <br>
lowercase_counter keeps track of how many lower case letters there are in a word. <br>
case_counter_list is an empty string that will evenutally hold the variables uppercase_counter and lowercase_counter. <br> 
<br>
3. Declare a for loop and if and else statements to identify capital or lowercase letters and update the counter variables:
```
for i in range(0, len(statement)): 
    if(statement[index_counter] == statement[index_counter].upper()): 
      uppercase_counter += 1 
    elif(statement[index_counter] == statement[index_counter].lower()): 
      lowercase_counter += 1 
    else: 
      uppercase_counter = uppercase_counter 
    index_counter += 1 
```
4. Append uppercase_counter and lowercase_counter to the list variable (case_counter_list):
```
case_counter_list.append(uppercase_counter) 
case_counter_list.append(lowercase_counter) 
```
5. Return the list from the function:
```
return case_counter_list 
```
6. Print the function:
```
sentence = input() 
sentence = str(sentence) 
print('UPPER CASE', lowerUpperCase(sentence)[0] ) 
print('LOWER CASE', lowerUpperCase(sentence)[1] ) 
```

# Q14 Solution
```
def lowerUpperCase(statement): 


  index_counter = 0 
  uppercase_counter = 0 
  lowercase_counter = 0 
  case_counter_list = [] 

  for i in range(0, len(statement)): 
    if(statement[index_counter] == statement[index_counter].upper()): 
      uppercase_counter += 1 
    elif(statement[index_counter] == statement[index_counter].lower()): 
      lowercase_counter += 1 
    else: 
      uppercase_counter = uppercase_counter 
    index_counter += 1 

  case_counter_list.append(uppercase_counter) 
  case_counter_list.append(lowercase_counter) 

  return case_counter_list 

sentence = input() 
sentence = str(sentence) 
print('UPPER CASE', lowerUpperCase(sentence)[0] ) 
print('LOWER CASE', lowerUpperCase(sentence)[1] ) 
```

# Question 15

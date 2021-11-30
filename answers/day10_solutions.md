# Question 31

# Q31 Task
Define a function which can print a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys.

# Q31 Procedure
1. Write a function:
```
def one_to_twenty_squares():
```
2. Declare an empty dictionary:
```
one_to_20_dictionary = {}
```
3. Use a for loop to add elements to the dictionary by using a declared variable:
```
one_to_20_dictionary = {}
num = 0
    
for i in range(0, 21):
  one_to_20_dictionary[num] = num * num
  num += 1
```
4. Return the dictionary:
```
return one_to_20_dictionary
```
5. Test the function:  
```
one_to_twenty_squares()
```
# Q31 Solution
```
def one_to_twenty_squares():
    
    one_to_20_dictionary = {}
    num = 0
    
    for i in range(0, 21):
        one_to_20_dictionary[num] = num * num
        num += 1
    
    return one_to_20_dictionary

one_to_twenty_squares()
```

# Question 32

# Q32 Task
Define a function which can generate a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys. The function should just print the keys only.

# Q32 Procedure
1. Write a function:
```
def one_to_twenty_squares():
```
2. Declare an empty dictionary:
```
one_to_20_dictionary = {}
```
3. Use a for loop to add elements to the dictionary by using a declared variable:
```
one_to_20_dictionary = {}
num = 0
    
for i in range(0, 21):
  one_to_20_dictionary[num] = num * num
  num += 1
```
4. Return the dictionary's keys:
```
return one_to_20_dictionary.keys()
```
5. Test the function:  
```
one_to_twenty_squares()
```

# Q32 Solution
```
def one_to_twenty_squares():
    
    one_to_20_dictionary = {}
    num = 0
    
    for i in range(0, 21):
        one_to_20_dictionary[num] = num * num
        num += 1
    
    return one_to_20_dictionary.keys()

one_to_twenty_squares()
```

# Question 33

# Q33 Task
Define a function which can generate and print a list where the values are square of numbers between 1 and 20 (both included).

# Q33 Procedure
1. Write a function:
```
def one_to_twenty_squares():
```
2. Declare an empty dictionary:
```
one_to_20_dictionary = {}
```
3. Use a for loop to add elements to the dictionary by using a declared variable and then append the dictionary's values to an empty list variable:
```
one_to_20_dictionary = {}
num = 0
list_of_values = []
    
for i in range(0, 21):
  one_to_20_dictionary[num] = num * num
  list_of_values.append(one_to_20_dictionary[num])
  num += 1
```
4. Return the list:
```
return list_of_values
```
5. Test the function:  
```
one_to_twenty_squares()
```

# Q33 Solution
```
def one_to_twenty_squares():
    
    one_to_20_dictionary = {}
    num = 0
    list_of_values = []
    
    for i in range(0, 21):
        one_to_20_dictionary[num] = num * num
        list_of_values.append(one_to_20_dictionary[num])
        num += 1
    
    return list_of_values

one_to_twenty_squares()
```

# Question 34

# Q34 Task
Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the first 5 elements in the list.

# Q34 Procedure
1. Make a function:
```
def one_to_20():
```
2. Within the function, assign a variable to an empty list:
```
list_of_nums = []
```
3. Use a for loop to find the square values from 1-20 and append them to the empty list:
```
num = 0
    
for i in range(0, 21):
  num_squ = num * num
  list_of_nums.append(num_squ)
  num +=1 
```
4. Return the first five elements in the list:
```
return list_of_nums[0], list_of_nums[1], list_of_nums[2], list_of_nums[3], list_of_nums[4]
```
5. Test the function:
```
one_to_20()
```
# Q34 Solution
```
def one_to_20():
    
    list_of_nums = []
    num = 0
    
    for i in range(0, 21):
        num_squ = num * num
        list_of_nums.append(num_squ)
        num +=1 
        
    return list_of_nums[0], list_of_nums[1], list_of_nums[2], list_of_nums[3], list_of_nums[4]
        
    
one_to_20()
```

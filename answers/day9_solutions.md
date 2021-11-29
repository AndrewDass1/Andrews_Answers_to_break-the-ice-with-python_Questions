# Day 9 Solutions

# Question 26

# Q26 Task
Define a function which can compute the sum of two numbers

# Q26 Procedure
1. Make the function:
```
def sum_of_two_numbers(num1, num2):
```
2. Return the sum:
```
def sum_of_two_numbers(num1, num2):
    return num1 + num2
```
3. Test the function:
```
sum_of_two_numbers(5,6)
```
# Q26 Solutions
```
def sum_of_two_numbers(num1, num2):
    return num1 + num2

sum_of_two_numbers(5,6)
```

# Question 27

# Q27 Task
Define a function that can convert an integer into a string and print it in the console

# Q27 Procedure 
1. Make the function:
```
def int_to_str():
```
2. Within the function, declare an integer and then cast the integer to a string:
```
def int_to_str():
  num = int(input(""))
  num_to_str = str(num)
```
3. Return the string:
```
return num_to_str, type(num_to_str)
```
type(num_to_str) is optional to include but running this statement verifies the variable is a string data type
4. Run the function:
```
int_to_str()
```

# Q27 Solution
```
def int_to_str():
    
    num = int(input(""))
    
    num_to_str = str(num)
    
    return num_to_str, type(num_to_str)

int_to_str()
```

# Question 28

# Q28 Task
Define a function that can receive two integer numbers in string form and compute their sum and then print it in console.

# Q28 Procedure
1. Make a function:
```
def add_string_numbers(num1, num2):
```
2. Cast the string variables to integers:
```
num1 = int(num1)
num2 = int(num2)
```
3. Return the sum of the casted integers:
```
return num1 + num2
```
4. Test the function:
```
add_string_numbers('5', '6')
```
# Q28 Solution
```
def add_string_numbers(num1, num2):

    num1 = int(num1)
    num2 = int(num2)
    
    return num1 + num2

add_string_numbers('5', '6')
```

# Question 29

# Q29 Task
Define a function that can accept two strings as input and concatenate them and then print it in console.

# Q29 Procedure 
1. Make a function:
```
def strings_concat():
```
2. Declare two string variables:
```
string1 = input()
string2 = input()
```
3. Return the concatenation of the two string variables:
```
return string1 + " " + string2
```
4. Test the function:
```
strings_concat()
```

# Q29 Solution
```
def strings_concat():
    
    string1 = input()
    string2 = input()
    
    return string1 + " " + string2

strings_concat()
```

# Question 30

# Q30 Task
Define a function that can accept two strings as input and print the string with maximum length in console. If two strings have the same length, then the function should print all strings line by line.

# Q30 Procedure
1. Make a function:
```
def string_compare():
```
2. Declare two variables to take two input strings and another variable to be an empty list:
```
str1 = input()
str2 = input()

str_list = []
```
3. Use if and else statements to return the string that has a larger length:
```
if len(str1) > len(str2):
        return str1
    elif len(str1) < len(str2):
        return str2
    else:
        str_list.append(str1)
        str_list.append(str2)
        return (print( str_list[0] + "\n" + str_list[1] ))
```
4. Run the function:
```
string_compare()
```

# Q30 Solution
```
def string_compare():
    str1 = input()
    str2 = input()
    
    str_list = []
    
    if len(str1) > len(str2):
        return str1
    elif len(str1) < len(str2):
        return str2
    else:
        str_list.append(str1)
        str_list.append(str2)
        return (print( str_list[0] + "\n" + str_list[1] ))

string_compare()
```

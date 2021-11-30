# Day 11 Solutions

# Question 38

# Q38 Task 
With a given tuple (1,2,3,4,5,6,7,8,9,10), write a program to print the first half values in one line and the last half values in one line.

# Q38 Procedure
1. Create a tuple that holds the values one to ten:
```
tuple_from_one_to_ten = (1,2,3,4,5,6,7,8,9,10)
```
2. Print the first five elements equally spaced from each other all on one line:
```
for i in range(0, 5):
    print(tuple_from_one_to_ten[num], end = ' ')
    num += 1

print('\n')
```
3. Print the last five elements equally spaced from each other all on one line:
```
for i in range(5,10):
    print(tuple_from_one_to_ten[num], end = ' ')
    num += 1
```

# Q38 Solution
```
tuple_from_one_to_ten = (1,2,3,4,5,6,7,8,9,10)
num = 0

for i in range(0, 5):
    print(tuple_from_one_to_ten[num], end = ' ')
    num += 1

print('\n')
    
for i in range(5,10):
    print(tuple_from_one_to_ten[num], end = ' ')
    num += 1
```

# Question 39

# Q39 Task
Write a program to generate and print another tuple whose values are even numbers in the given tuple (1,2,3,4,5,6,7,8,9,10).

# Q39 Procedure
1. Make a tuple that has the numbers one to ten:
```
tuple_one_to_ten = (1,2,3,4,5,6,7,8,9,10)
```
2. By using a for loop, go through the tuple's indexes to see which numbers are even by using an if and else statement and the modulus operator. In the process, append the even numbers to a list variable:
```
num_index = 0
nums_div_by_2 = []

for i in range(0, len(tuple_one_to_ten)):
    if tuple_one_to_ten[num_index] % 2 == 0:
        nums_div_by_2.append(tuple_one_to_ten[num_index])
    num_index += 1
```
3. Print the result:
```
print(nums_div_by_2)
```

# Q39 Solution
```
tuple_one_to_ten = (1,2,3,4,5,6,7,8,9,10)
num_index = 0
nums_div_by_2 = []

for i in range(0, len(tuple_one_to_ten)):
    if tuple_one_to_ten[num_index] % 2 == 0:
        nums_div_by_2.append(tuple_one_to_ten[num_index])
    num_index += 1
    
print(nums_div_by_2)
```

# Question 40

# Q40 Task
Write a program which accepts a string as input to print "Yes" if the string is "yes" or "YES" or "Yes", otherwise print "No".

# Q40 Procedure 
1. Declare a variable to take an input:
```
decision = input("")
```
2. Use an if and else statement to check whether yes, Yes, or YES was inputted to print back out 'Yes' and 'No' for every other response:
```
if decision == "yes" or decision == "Yes" or decision == "YES":
    print("Yes")
else:
    print("No")
```

# Q40 Solution
```
decision = input("")

if decision == "yes" or decision == "Yes" or decision == "YES":
    print("Yes")
else:
    print("No")
```

# Question 41

# Q41 Task
Write a program which can map() to make a list whose elements are square of elements in [1,2,3,4,5,6,7,8,9,10].

# Q41 Procedure
1. Write a function to multiply two numbers:
```
def multiply(num):
    return num*num
```
2. Declare two variables one to hold an empty list and the other set to 0:
```
list_of_nums = [] 
add_num_to_list = 0
```
3. By using a for loop to run in the range 0 to 11, the variable add_num_to_list can be appended to the empty list variable to add numbers 0 to 10 to the list:
```
for i in range(0, 11):
    list_of_nums.append(add_num_to_list)
    add_num_to_list += 1
```
4. Declare a variable to use the map function to find the square values of the list of numbers:
```
elements_squ = map(multiply, list_of_nums)
```
The map function takes two variables in the parenthesis: a function and then a data type. It follows the function's rules and applies them to the data type that was given.  <br>
<br>
In this case, the function returns the square value of any number given to it. Since the list contains numbers 1 to 10, the map function will use the multiply function to return the square values of every number. <br>
<br>
5. Print the list of elements:
```
print(list(elements_squ))
```


# Q41 Solution
```
def multiply(num):
    return num*num

list_of_nums = [] 
add_num_to_list = 0

for i in range(0, 11):
    list_of_nums.append(add_num_to_list)
    add_num_to_list += 1
    
elements_squ = map(multiply, list_of_nums)

print(list(elements_squ))
```

# Question 42

# Q42 Task
Write a program which can map() and filter() to make a list whose elements are square of even number in [1,2,3,4,5,6,7,8,9,10].

# Q42 Procedure
1. Create a multiply function:
```
def multiply(num):
    return num*num
```
2. Create a function to return numbers that are divisible by 2:
```
def num_check_div_by_2(num):
    if num % 2 == 0:
        return num
```
3. Create a list containing the numbers one to ten:
```
list_one_to_ten = [1,2,3,4,5,6,7,8,9,10]
```
4. Declare a variable to use the map and filter functions to find every even number and then square the even values:
```
even_nums = map(multiply, filter(num_check_div_by_2, list_one_to_ten))
```
The filter function syntax works in a similar way to the map function. <br>
<br>
5. Print the list of even numbers:
```
print(list(even_nums))
```
# Q42 Solution
def multiply(num):
    return num*num
    
def num_check_div_by_2(num):
    if num % 2 == 0:
        return num
    
list_one_to_ten = [1,2,3,4,5,6,7,8,9,10]

even_nums = map(multiply, filter(num_check_div_by_2, list_one_to_ten))
print(list(even_nums))

# Question 43

# Q43 Task
Write a program which can filter() to make a list whose elements are even number between 1 and 20 (both included).

# Q43 Procedure
1. Create a function to see if numbers are divisible by 2:
```
def even_number(num):
  if num % 2 == 0:
    return num
```
2. Assign a variable to be an empty list:
```
list_one_to_20 = []
```
3. Use a for loop to append numbers 1 to 20 to the list:
```
for i in range(0, 21):
  list_one_to_20.append(num)
  num += 1
```
4. Use the filter function to find the even numbers in the list:
```
list_even_numbers = filter(even_number, list_one_to_20)
```
5. Print the variable that contains the filter function:
```
print(list (list_even_numbers) )
```
# Q43 Solution
```
def even_number(num):
  if num % 2 == 0:
    return num

list_one_to_20 = []
num = 0

for i in range(0, 21):
  list_one_to_20.append(num)
  num += 1
    
list_even_numbers = filter(even_number, list_one_to_20)
print(list (list_even_numbers) )
```

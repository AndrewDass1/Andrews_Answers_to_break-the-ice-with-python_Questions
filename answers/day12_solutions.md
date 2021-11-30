# Day 12 Solutions

# Question 44

# Q44 Task
Write a program which can map() to make a list whose elements are square of numbers between 1 and 20 (both included).

# Q44 Procedure
1. Make a function to return the square value of an integer:
```
def square_number(num):
  return num * num
```
2. Declare a list data type:
```
list_one_to_20 = []
```
3. Use a for loop to add elements to the list:
```
num = 0

for i in range(0, 21):
    list_one_to_20.append(num)
    num += 1
```
4. Use the map function to receive square values of the list's integers:
```
list_even_numbers = map(square_number, list_one_to_20)
```
5. Print the final result:
```
print(list (list_even_numbers) )
```

# Q44 Solution
```
def square_number(num):
    return num * num

list_one_to_20 = []
num = 0

for i in range(0, 21):
    list_one_to_20.append(num)
    num += 1
    
list_even_numbers = map(square_number, list_one_to_20)
print(list (list_even_numbers) )
```

# Question 45

# Q45 Task
Define a class named American which has a static method called printNationality.

# Q45 Procedure
1. Create a class:
```
class American:
```
2. Make a static method or a function called printNationality:
```
class American:
    def printNationality(ask_nationality):
        ask_nationality = input("")
        return ask_nationality
```
3. Test the class out my assigning the class to a variable and then print the variable:
```
hello_I_am = American()
print(hello_I_am.printNationality())
```

# Q45 Solution
```
class American:
    def printNationality(ask_nationality):
        ask_nationality = input("")
        return ask_nationality
        
hello_I_am = American()
print(hello_I_am.printNationality())
```

# Question 46 

# Q46 Task
Define a class named American and its subclass NewYorker.

# Q46 Procedure
1. Create the American and NewYorker classes:
```
class American():
    None
    
class NewYorker():
    None
```
2. Assign the classes to variables:
```
nationality = American()
resident = NewYorker() 
```
3. Test out the classes by printing the variables:
```
print(nationality)
print(resident)
```
# Q46 Solution
```
class American():
    None
    
class NewYorker():
    None
    
nationality = American()
resident = NewYorker() 

print(nationality)
print(resident)
```

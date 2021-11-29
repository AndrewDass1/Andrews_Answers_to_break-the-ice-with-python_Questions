# Day 8 Solutions

# Question 22

# Q22 Task
Write a program to compute the frequency of the words from the input. The output should output after sorting the key alphanumerically. <br>
<br>
Suppose the following input is supplied to the program:
```
New to Python or choosing between Python 2 and Python 3? Read Python 2 or Python 3.
```
Then the output should be:
```
2:2
3.:1
3?:1
New:1
Python:5
Read:1
and:1
between:1
choosing:1
or:2
to:1
```

# Q22 Procedure 
1. Make a function:
```
def word_frequency():    
```
2. Declare variables:
```
statement = input("").split()
statement_words = list(set(statement))
same_word_counter = 0
same_word_counter_list = []
    
index = 0
index2 = 0
index3 = 0
```
statement takes a string input but every index is separated by the split function <br>
statement_words is the statement variable that is casted by the set data type to remove any duplicates <br>
<br>
By having the original list and a set of no duplicates, they can be compared with one another by using a for loop and variables specified as counters to keep track of what and how many times the same words appeared. <br>
<br>
same_word_counter is the variable to keep track of the same word <br>
same_word_counter_list receives the same word counter after the value is appended to it <br>

3. Use a for and while loops to go through the two list and set, check for how many times what and each words appeared by updating the same word counter:
```
for i in range(0, len(statement_words)):
  index = 0
  same_word_counter = 0
        
  while (index < len(statement)):
    if(statement[index] == statement_words[index2]):
      same_word_counter += 1
                
    index += 1
            
  same_word_counter_list.append(same_word_counter)
  index2 += 1
    
    
for i in range(0, len(statement_words)):  
  print(statement_words[index3],":",same_word_counter_list[index3] )
        
  index3 += 1
```
4. Run the function:  
```
word_frequency()
```
# Q22 Solution
```
def word_frequency():
    
    statement = input("").split()
    statement_words = list(set(statement))
    same_word_counter = 0
    same_word_counter_list = []
    
    dictionary = {}
    
    index = 0
    index2 = 0
    index3 = 0
    
    for i in range(0, len(statement_words)):
        index = 0
        same_word_counter = 0
        
        while (index < len(statement)):
            if(statement[index] == statement_words[index2]):
                same_word_counter += 1
                
            index += 1
            
        same_word_counter_list.append(same_word_counter)
        index2 += 1
    
    
    for i in range(0, len(statement_words)):  
        print(statement_words[index3],":",same_word_counter_list[index3] )
        
        index3 += 1
```

# Question 23

# Q23 Task
Write a method which can calculate square value of number

# Q23 Procedure
1. Write a function:
```
def square_a_number():
```
2. Declare an integer data type:
```
def square_a_number():
  num = int(input(""))
```
3. Return the square value of num:
```
def square_a_number():
  num = int(input(""))
  return num * num
```
4. Run the function:
```
return square_a_number()
```

# Q23 Solution
```
def square_a_number():
  num = int(input(""))
  return num * num

square_a_number()
```

# Question 24

# Q24 Task
Python has many built-in functions, and if you do not know how to use it, you can read document online or find some books. But Python has a built-in document function for every built-in functions. <br>
<br>
Please write a program to print some Python built-in functions documents, such as abs(), int(), raw_input() <br>
<br>
And add document for your own function
# Q24 Procedure
1. Write a function:
```
def abs_integer():

```
2. Declare a variable to be a float data type:
```
num = float(input(""))
```
3. Cast num or the variable holding the float data type with abs() and int() as shown below:
```
int_num = abs(int(num))
```
It seems its contradictory to first declare a float just to cast it as integer, however, by using a float, the user can input decimal answers and the program will output its absolute value integer to the nearest 0. <br>
<br>
4. Return int_num or the variable that holds the absolute value integer:
```
return int_num
```
5. Run the function:
```
abs_integer()
```
# Q24 Solution
```
def abs_integer():
    
    num = float(input(""))
    
    int_num = abs(int(num))
    
    return int_num

abs_integer()
```

# Question 25

# Q25 Task
Define a class, which have a class parameter and have a same instance parameter.

# Q25 Procedure
1. Make a class:
```
class tutorial:
```
2. Write a function:
```
def __init__(self,name,age):
        
  self.name = None
  self.age = age
```
3. Test out the class:
```
testing_the_class.name = 'John'
testing_the_class2.name = 'Bob'
```
4. Print out the variables to test the class:
```
print(testing_the_class.name)
print(testing_the_class2.name)
```

# Q25 Solution
```
class tutorial:
    
    def __init__(self,name,age):
        
        self.name = None
        self.age = age

testing_the_class.name = 'John'
testing_the_class2.name = 'Bob'
        

print(testing_the_class.name)
print(testing_the_class2.name)
```

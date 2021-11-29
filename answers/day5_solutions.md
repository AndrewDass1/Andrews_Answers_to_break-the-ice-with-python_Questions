# Day 5 Solutions

# Question 16

# Q16 Task
Use a list comprehension to square each odd number in a list. The list is input by a sequence of comma-separated numbers. >Suppose the following input is supplied to the program:
```
1,2,3,4,5,6,7,8,9
```
The, the output showed be:
```
1,9,25,49,81
```

# Q16 Procedure
1. #Specify to numbers to ask for, one number being the lower limit and the next number being the higher limit
```
lower_range = int(input(""))
higher_range = int(input(""))
```
2. The problem asks to store the numbers between and including the lower and higher limit in a list. To declare a list, we need to define one as shown below:
```
list_of_numbers = []
```
Though list_of_numbers is empty, it is possible to add elements in the empty list by using the append command <br>
3. By having the lower and higher limits specified as variables, it is possible to shuffle through the indexes by declaring a index counter and by using a for loop in order to add numbers in list_of_numbers:
```
for i in range(lower_range, higher_range+1):
  list_of_numbers.append(number_increment)
  number_increment +=1
```
4. Declare variables, use a while loop and several if statements to create lists to:
* First hold the list of values
* Another list to hold the square values of the odd numbers

```
index_counter = 0
index_counter2 = 0
index_counter3 = 0
num_odd_square_list = []

while (index_counter < len(list_of_numbers)):
  if(list_of_numbers[index_counter] % 2 != 0):
    odd_squared = list_of_numbers[index_counter] ** 2
    num_odd_square_list.append(odd_squared)
  index_counter += 1
```

To print the original list though it is not required:
```
for i in range(0, len(list_of_numbers)-1):
  print(list_of_numbers[index_counter2], end=',')
  index_counter2+=1
print(list_of_numbers[len(list_of_numbers) -1 ])
```

```
for i in range(0, len(num_odd_square_list)-1):
  print(num_odd_square_list[index_counter3], end=',')
  index_counter3 += 1
```


# Q16 Solution
```
lower_range = int(input(""))
higher_range = int(input(""))

list_of_numbers = []

number_increment = lower_range

for i in range(lower_range, higher_range+1):
#in range(,+1) to ensure it reaches higher_range)
  list_of_numbers.append(number_increment)
  number_increment +=1

index_counter = 0
index_counter2 = 0
index_counter3 = 0
num_odd_square_list = []

while (index_counter < len(list_of_numbers)):
  if(list_of_numbers[index_counter] % 2 != 0):
    odd_squared = list_of_numbers[index_counter] ** 2
    num_odd_square_list.append(odd_squared)
  index_counter += 1
  
for i in range(0, len(list_of_numbers)-1):
  print(list_of_numbers[index_counter2], end=',')
  index_counter2+=1
print(list_of_numbers[len(list_of_numbers) -1 ])

for i in range(0, len(num_odd_square_list)-1):
  print(num_odd_square_list[index_counter3], end=',')
  index_counter3 += 1

print(num_odd_square_list[len(num_odd_square_list) -1] )
```

# Question 17

# Q17 Task
Write a program that computes the net amount of a bank account based a transaction log from console input. The transaction log format is shown as following:
```
D 100
W 200
```
D means deposit while W means withdrawal <br>
<br>
Suppose the following input is supplied to the program:
```
D 300
D 300
W 200
D 100
```
Then, the output should be:
```
500
```
# Q17 Procedure
1. Declare a function and within the function, a variable to take an integer data type:
```
def bankActions():

  actions = int(input(""))
```
2. Use the integer data type to make a "for i in range(0, int_data_type). This will run the program as much times the user specified once before thanks to the integer variable and the range() function.  
```
  total = 0
  for i in range(0, actions):
    choice = input()
```
Total is the total amount of money that is left from all the deposits and withdrawals. <br>
<br>
3. Create if and else statements to either deposit or withdraw money:
```
if choice == 'D':
      deposit = float(input(""))
      total = total + deposit

    elif choice == 'W':
      withdraw = float(input(""))
      total = total - withdraw

    else:
      print('Invalid')
```
4. Return total:
```
return total
```
5. Run the function:
```
bankActions()
```
# Q17 Solution

```
#Q17

def bankActions():


  actions = int(input(""))
  total = 0

  for i in range(0, actions):
    choice = input()

    if choice == 'D':
      deposit = float(input(""))
      total = total + deposit

    elif choice == 'W':
      withdraw = float(input(""))
      total = total - withdraw

    else:
      print('Invalid')

  return total
  
    
bankActions()
```

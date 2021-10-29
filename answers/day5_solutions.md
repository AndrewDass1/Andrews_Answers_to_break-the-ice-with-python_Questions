# Day 5 Solutions

# Question 16
```
#Specify to numbers to ask for, one number being the lower limit and the next number being the higher limit

lower_range = int(input(""))
higher_range = int(input(""))

#The problem asks to store the numbers between and including the lower and higher limit in a list.
#To declare a list, we need to define one as shown below:

list_of_numbers = []

#Though list_of_numbers is empty, it is possible to add elements in the empty list by using the append command

#By having the lower and higher limits specified as variables, it is possible to shuffle through the indexes by declaring a index counter and by using a for loop in order to add
#numbers in list_of_numbers

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

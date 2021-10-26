# Day 2 Solutions

# Question 4
num = int(input(""))
list_of_num = []

for i in range(0, num):
  enter_num = int(input(""))
  list_of_num.append(enter_num)

num_tuple = tuple(list_of_num)
print(num_tuple)

# Question 5

# Question 6
C = 50
D = int(input(""))
H = 30

Q = ((2*C*D)/H) ** (1/2)
print(Q)

# Question 7
listarray = []
numdim = int(input(""))
numenter = int(input(""))

for i in range(0, numdim):
  listarray.append([])

<!--for i2 in range(0, len(listarray))-->

print(listarray)
print(len(listarray))
print((listarray[1]))

# Question 8
statement = input("").split(",")
num_counter = 0
sorted_statement = sorted(statement)

#Split shows if the statement is separated by , then it will be sorted

for i in range(0, len(statement)):
  print(sorted_statement[num_counter], end=" ")
  num_counter += 1
  
# Question 9
num_of_statements = int(input(""))
statementlist = []
num_counter = 0

for i in range(0, num_of_statements):
  statement = input("").upper()
  statementlist.append(statement)

for i2 in range(0, num_of_statements):
  print(statementlist[num_counter])
  num_counter += 1

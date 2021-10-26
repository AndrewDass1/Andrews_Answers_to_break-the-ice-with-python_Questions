# Day 2 Solutions

# Question 4
num = int(input("")) <br>
list_of_num = [] <br>br>

for i in range(0, num): <br>
  enter_num = int(input("")) <br>
  list_of_num.append(enter_num) <br>

num_tuple = tuple(list_of_num) <br>
print(num_tuple) <br>

# Question 5

# Question 6
C = 50 <br>
D = int(input("")) <br>
H = 30 <br>

Q = ((2* C *D) / H) ** (1/2) <br>
print(Q) <br>

With a Function: <br>
def math_formula(): <br>

  C = 50 <br>
  D = int(input("")) <br>
  H = 30 <br>

  Q = ((2 * C * D) / H) ** (1/2) <br>
  return(Q) <br>

math_formula()

# Question 7


# Question 8
statement = input("").split(",") <br>
num_counter = 0 <br>
sorted_statement = sorted(statement) <br>

#Split shows if the statement is separated by , then it will be sorted

for i in range(0, len(statement)): <br>
  print(sorted_statement[num_counter], end=" ") <br>
  num_counter += 1 <br>
  
# Question 9
num_of_statements = int(input("")) <br>
statementlist = [] <br>
num_counter = 0 <br>

for i in range(0, num_of_statements): <br>
  statement = input("").upper() <br>
  statementlist.append(statement) <br>

for i2 in range(0, num_of_statements): <br>
  print(statementlist[num_counter]) <br>
  num_counter += 1 <br>

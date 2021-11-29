# Day 6 Solutions

# Question 18

# Q18 Task
A website requires the users to input username and password to register. Write a program to check the validity of password input by users. <br>
<br>
Following are the criteria for checking the password: <br>
* At least 1 letter between [a-z]
* At least 1 number between [0-9]
* At least 1 letter between [A-Z]
* At least 1 character from [$#@]
* Minimum length of transaction password: 6
* Maximum length of transaction password: 12 <br>
<br>

Your program should accept a sequence of comma separated passwords and will check them according to the above criteria. 
Passwords that match the criteria are to be printed, each separated by a comma. <br>
<br>
Example <br>
If the following passwords are given as input to the program:
```
ABd1234@1,a F1#,2w3E*,2We3345
```
Then, the output of the program should be:
```
ABd1234@1
```

# Q18 Procedure
1. Create a function:
```
def enter_password():
```

2. Within the function declare a variable to take a string and other variable counters to keep track of lowercase letters, uppercase letters, number counters and character counters:
```
def enter_password():
    
    statement = input('')
    
    check_index_criteria = 0
    
    lower_letter_counter = 0
    number_counter = 0
    upper_letter_counter = 0
    character_counter = 0
```
3. Use a for loop to go through the string's indexes to see what it contains and if and else statements to update the counters:
```
    for i in range(0, len(statement)):
        if (statement[check_index_criteria] == '0' or statement[check_index_criteria] == '1' or statement[check_index_criteria] == '2' or statement[check_index_criteria] == '3' or statement[check_index_criteria] == '4' or statement[check_index_criteria] == '5' or statement[check_index_criteria] == '6' or statement[check_index_criteria] == '7' or statement[check_index_criteria] == '8' or statement[check_index_criteria] == '9'   ):
            number_counter += 1
        elif(statement[check_index_criteria] == '$' or statement[check_index_criteria] == '#' or statement[check_index_criteria] == '@'):
            character_counter += 1
        elif (statement[check_index_criteria] == statement[check_index_criteria].lower()):
            lower_letter_counter += 1
        elif (statement[check_index_criteria] == statement[check_index_criteria].upper()):
            upper_letter_counter += 1
        else:
            number_counter = number_counter
            
        check_index_criteria += 1
```

4. Use another if and else statement to see if the password meets all the requirements, return the password from the function:
```
if ( (len(statement) >= 6 or len(statement) <= 12) and number_counter > 0 and lower_letter_counter > 0 and upper_letter_counter > 0 and character_counter > 0):
        return statement
    else:
        error_statement2 = 'The password does not meet the requirements. Try again.'
        return error_statement2
```
# Q18 Solution
```
def enter_password():
    
    statement = input('')
    
    check_index_criteria = 0
    
    lower_letter_counter = 0
    number_counter = 0
    upper_letter_counter = 0
    character_counter = 0
        
    for i in range(0, len(statement)):
        if (statement[check_index_criteria] == '0' or statement[check_index_criteria] == '1' or statement[check_index_criteria] == '2' or statement[check_index_criteria] == '3' or statement[check_index_criteria] == '4' or statement[check_index_criteria] == '5' or statement[check_index_criteria] == '6' or statement[check_index_criteria] == '7' or statement[check_index_criteria] == '8' or statement[check_index_criteria] == '9'   ):
            number_counter += 1
        elif(statement[check_index_criteria] == '$' or statement[check_index_criteria] == '#' or statement[check_index_criteria] == '@'):
            character_counter += 1
        elif (statement[check_index_criteria] == statement[check_index_criteria].lower()):
            lower_letter_counter += 1
        elif (statement[check_index_criteria] == statement[check_index_criteria].upper()):
            upper_letter_counter += 1
        else:
            number_counter = number_counter
            
        check_index_criteria += 1
    
    print(lower_letter_counter)
    print(number_counter)
    print(upper_letter_counter)
    print(character_counter)
    
    if ( (len(statement) >= 6 or len(statement) <= 12) and number_counter > 0 and lower_letter_counter > 0 and upper_letter_counter > 0 and character_counter > 0):
        return statement
    else:
        error_statement2 = 'The password does not meet the requirements. Try again.'
        return error_statement2

```

# Question 19

# Q19 Task
You are required to write a program to sort the (name, age, score) tuples by ascending order where name is string, age and score are numbers. The tuples are input by console. The sort criteria is:
* 1: Sort based on name
* 2: Then sort based on age
* 3: Then sort by score <br>
<br>
The priority is that name > age > score <br>
<br>
If the following tuples are given as input to the program:
```
Tom,19,80
John,20,90
Jony,17,91
Jony,17,93
Json,21,85
```
Then, the output of the program should be:
```
[('John', '20', '90'), ('Jony', '17', '91'), ('Jony', '17', '93'), ('Json', '21', '85'), ('Tom', '19', '80')]
```

# Q19 Procedure
1. Create a function:
```
def name_Age_Score():
```
2. Declare an integer data type and a empty list:
```
entries = int(input(""))
list_of_info = []
```
3. Use the declare data type to make a for in range(0, int data type variable) to run the program as much times to input many people's names, ages and scores:
```
for i in range(0, entries):
  name = input("")
  age = int(input(""))
  score = input("")
```
4. Create a tuple of the name, age and score variables:
```
tuple_of_info = (name,age,score)
```
5. Append tuple_of_info to the empty list:
```
list_of_info.append(tuple_of_info)
```
6. Return the sorted list of people's information:    
```
return sorted(list_of_info)
```
7. Run the function:
```
name_Age_Score()
```
# Q19 Solution
```
def name_Age_Score():
    
    entries = int(input(""))
    list_of_info = []
    
    for i in range(0, entries):

        
        name = input("")
        age = int(input(""))
        score = input("")
        
        tuple_of_info = (name,age,score)
        list_of_info.append(tuple_of_info)
    
    return sorted(list_of_info)
    
name_Age_Score() 
```

# Day 3 Solutions

# Question 10

# Q10 Task
Write a program that accepts a sequence of whitespace separated words as input and prints the words after removing all duplicate words and sorting them alphanumerically. <br>
<br>
Suppose the following input is supplied to the program:
```
hello world and practice makes perfect and hello world again
```
Then, the output should be:
```
again and hello makes perfect practice world
```

# Q10 Procedure
1. Declare a variable to input any statement that each word is separated by a space
```
statement = input("").split(" ")
```
2. Cast the variable that contains the phrase to a set data type sort the sentence in alphabetical order and to remove any duplicate words:
```
no_repeated_word_statement = set(statement)
```
3. Print the statement in alphabetical order on one line:
```
no_repeated_word_statement = list(no_repeated_word_statement)
num_counter = 0

for i in range(0, len(no_repeated_word_statement)):
  print(no_repeated_word_statement[num_counter], end=" ")
  num_counter += 1
```
End = " " within the print makes sure the index of 'no_repeated_word_statement[num_counter] is printed on the same line since ' end = " " ' specifies each term that is outputted by the for loop will be separated by a space. 

# Q10 Solution
```
statement = input("").split(" ")
no_repeated_word_statement = set(statement)
no_repeated_word_statement = list(no_repeated_word_statement)
num_counter = 0

for i in range(0, len(no_repeated_word_statement)):
  print(no_repeated_word_statement[num_counter], end=" ")
  num_counter += 1
```

# Question 11


# Question 12

# Q12 Task
Write a program, which will find all such numbers between 1000 and 3000 (both included) such that each digit of the number is an even number.The numbers obtained should be printed in a comma-separated sequence on a single line.

# Q12 Procedure
1. Declare a variable to be equal to 1000:
```
current_value = 1000
```
2. Write a for loop to run in the limit from 1000 to 3000:
```
for i in range(1000, 3001):
```
3. The for loop is responsible to index all of the numbers digits. <br>
<br>
   For example, if the number is 1013, we need to see if all the digits: 1, 0, 1, and 3 are all even. Therefore each index of every number from 1000 to 3000 must    be checked. An integer does not have any indexesm therefore the declare integer variable must be casted to a string and to check every index of the number. 
```
string_current_value = str(current_value)
digit0 = (str(current_value))[0]
digit1 = (str(current_value))[1]
digit2 = (str(current_value))[2]
digit3 = (str(current_value))[3]
```
4. Use an if and else statements to find the numbers between 1000 to 3000 that have all even digits and print every number on one line:
```
if int(digit0) % 2 == 0 and int(digit1) % 2 == 0 and int(digit2) % 2 == 0 and int(digit3) % 2 == 0:
    print(current_value, end=" ")
  current_value +=1
```

# Q12 Solution 
```
current_value = 1000

for i in range(1000, 3001):
  string_current_value = str(current_value)
  digit0 = (str(current_value))[0]
  digit1 = (str(current_value))[1]
  digit2 = (str(current_value))[2]
  digit3 = (str(current_value))[3]

  if int(digit0) % 2 == 0 and int(digit1) % 2 == 0 and int(digit2) % 2 == 0 and int(digit3) % 2 == 0:
    print(current_value, end=" ")
  current_value +=1
```

# Question 13

# Q13 Task
Write a program that accepts a sentence and calculate the number of letters and digits. <br>
<br>
Suppose the following input is supplied to the program:
```
hello world! 123
```
Then, the output should be:
```
LETTERS 10
DIGITS 3
```

# Q13 Procedure
1. Declare a variable that takes a string <br>
<br>
   Below I wrote a function to incorporate my code:
```
def digitletterCounter(sentence):
```
2. Integrate for loops and if and else statements together to keep track of the amount of letters and numbers from the string variable. Declare other variables as needed to complete the task. Below are the additional variables that was created:
```
index_position = 0 
letter_counter = 0
number_counter = 0
counter_values = []
```
Index position is reponsible for going through each index of the string variable. <br>
Letter counter is updated after how much letters is detected in the string. <br>
Number counter is updated after how much numbers is detected in the string. <br>
Counter_values is an empty list that will eventually hold the letter_counter and number_counter variables to show the total number of letters and numbers.  <br>

3. Create the for loop and if and else statements:
```
for i in range(0, len(sentence)):
    if sentence[index_position] == '0' or sentence[index_position] == '1' or sentence[index_position] == '2' or sentence[index_position] == '3' or sentence[index_position] == '4' or sentence[index_position] == '5' or sentence[index_position] == '6' or sentence[index_position] == '7' or sentence[index_position] == '8' or sentence[index_position] == '9':
      number_counter = number_counter + 1
    elif sentence[index_position] >= 'a' or sentence[index_position] >= 'A' or sentence[index_position] <= 'z' or sentence[index_position] <= 'Z':
      letter_counter = letter_counter + 1
    else:
      number_counter = number_counter
    index_position = index_position + 1
```
4. Append letter_counter and number_counter to an empty list (in this case the empty list is called counter_values):
```
counter_values.append(letter_counter)
counter_values.append(number_counter)
```
5. Since this is a function, a variable must be returned. In this case, counter values now holds both letter_counter and number_counter which needs to be returned:
```
return counter_values
```
6. Run the function:
```
#Testing the function 
words_and_letters = input() 
words_and_letters = str(words_and_letters) 

print('LETTERS',digitletterCounter(words_and_letters)[0]) 
print('DIGITS',digitletterCounter(words_and_letters)[1])
```

# Q13 Solution
```
def digitletterCounter(sentence):
  
  
  index_position = 0 
  letter_counter = 0
  number_counter = 0
  counter_values = []
  
  for i in range(0, len(sentence)):
    if sentence[index_position] == '0' or sentence[index_position] == '1' or sentence[index_position] == '2' or sentence[index_position] == '3' or sentence[index_position] == '4' or sentence[index_position] == '5' or sentence[index_position] == '6' or sentence[index_position] == '7' or sentence[index_position] == '8' or sentence[index_position] == '9':
      number_counter = number_counter + 1
    elif sentence[index_position] >= 'a' or sentence[index_position] >= 'A' or sentence[index_position] <= 'z' or sentence[index_position] <= 'Z':
      letter_counter = letter_counter + 1
    else:
      number_counter = number_counter
    index_position = index_position + 1
  
  counter_values.append(letter_counter)
  counter_values.append(number_counter)
  
  return counter_values
  
  
#Testing the function 
words_and_letters = input() 
words_and_letters = str(words_and_letters) 

print('LETTERS',digitletterCounter(words_and_letters)[0]) 
print('DIGITS',digitletterCounter(words_and_letters)[1]) 
```



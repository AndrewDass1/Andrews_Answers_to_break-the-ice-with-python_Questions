# Day 3 Solutions

# Question 10
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

# Question 14
```
def lowerUpperCase(statement):


  index_counter = 0 
  uppercase_counter = 0 
  lowercase_counter = 0 
  case_counter_list = [] 
  
  for i in range(0, len(statement)): 
    if(statement[index_counter] == statement[index_counter].upper()): 
      uppercase_counter += 1 
    elif(statement[index_counter] == statement[index_counter].lower()): 
      lowercase_counter += 1 
    else: 
      uppercase_counter = uppercase_counter 
    index_counter += 1 
  
  case_counter_list.append(uppercase_counter) 
  case_counter_list.append(lowercase_counter) 

  return case_counter_list 

sentence = input() 
sentence = str(sentence) 
print('UPPER CASE', lowerUpperCase(sentence)[0] ) 
print('LOWER CASE', lowerUpperCase(sentence)[1] ) 
```

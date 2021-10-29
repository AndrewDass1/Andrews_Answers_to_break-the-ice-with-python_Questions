# Day 3 Solutions

# Question 10
statement = input("").split(" ") <br>
no_repeated_word_statement = set(statement) <br>
no_repeated_word_statement = list(no_repeated_word_statement) <br>
num_counter = 0 <br>
<br>
for i in range(0, len(no_repeated_word_statement)): <br>
  print(no_repeated_word_statement[num_counter], end=" ") <br>
  num_counter += 1
  
# Question 11


# Question 12
current_value = 1000 <br>

for i in range(1000, 3001): <br>
  string_current_value = str(current_value) <br>
  digit0 = (str(current_value))[0] <br>
  digit1 = (str(current_value))[1] <br>
  digit2 = (str(current_value))[2] <br>
  digit3 = (str(current_value))[3] <br>

  if int(digit0) % 2 == 0 and int(digit1) % 2 == 0 and int(digit2) % 2 == 0 and int(digit3) % 2 == 0: <br>
    print(current_value, end=" ") <br>
  current_value +=1

# Question 13
def digitletterCounter(sentence): <br>
  <br>
  <br>
  index_position = 0 <br>
  letter_counter = 0 <br>
  number_counter = 0 <br>
  counter_values = [] <br>
  <br>
  for i in range(0, len(sentence)): <br>
    if sentence[index_position] == '0' or sentence[index_position] == '1' or sentence[index_position] == '2' or sentence[index_position] == '3' or sentence[index_position] == '4' or sentence[index_position] == '5' or sentence[index_position] == '6' or sentence[index_position] == '7' or sentence[index_position] == '8' or sentence[index_position] == '9': <br>
      number_counter = number_counter + 1 <br>
    elif sentence[index_position] >= 'a' or sentence[index_position] >= 'A' or sentence[index_position] <= 'z' or sentence[index_position] <= 'Z': <br>
      letter_counter = letter_counter + 1 <br>
    else: <br>
      number_counter = number_counter <br>
    index_position = index_position + 1 <br>
  <br>
  counter_values.append(letter_counter) <br>
  counter_values.append(number_counter) <br>
  <br>
  return counter_values <br>
  <br>
  <br>
#Testing the function <br>
words_and_letters = input() <br>
words_and_letters = str(words_and_letters) <br>
<br>
print('LETTERS',digitletterCounter(words_and_letters)[0]) <br>
print('DIGITS',digitletterCounter(words_and_letters)[1]) <br>

# Question 14
def lowerUpperCase(statement): <br>
<br>
<br>
  index_counter = 0 <br>
  uppercase_counter = 0 <br>
  lowercase_counter = 0 <br>
  case_counter_list = [] <br>
  <br>
  for i in range(0, len(statement)): <br>
    if(statement[index_counter] == statement[index_counter].upper()): <br>
      uppercase_counter += 1 <br>
    elif(statement[index_counter] == statement[index_counter].lower()): <br>
      lowercase_counter += 1 <br>
    else: <br>
      uppercase_counter = uppercase_counter <br>
    index_counter += 1 <br>
  <br>
  case_counter_list.append(uppercase_counter) <br>
  case_counter_list.append(lowercase_counter) <br>

  return case_counter_list <br>

sentence = input() <br>
sentence = str(sentence) <br>
print('UPPER CASE', lowerUpperCase(sentence)[0] ) <br>
print('LOWER CASE', lowerUpperCase(sentence)[1] ) 

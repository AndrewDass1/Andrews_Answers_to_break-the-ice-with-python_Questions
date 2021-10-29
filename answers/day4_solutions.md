# Day 4 Solutions

# Question 14
def lowerUpperCase(statement): <br>
<br>
<br>
  index_counter = 0 <br>
  uppercase_counter = 0 <br>
  lowercase_counter = 0 <br>
  case_counter_list = [] <br>

  for i in range(0, len(statement)): <br>
    if(statement[index_counter] == statement[index_counter].upper()): <br>
      uppercase_counter += 1 <br>
    elif(statement[index_counter] == statement[index_counter].lower()): <br>
      lowercase_counter += 1 <br>
    else: <br>
      uppercase_counter = uppercase_counter <br>
    index_counter += 1 <br>

  case_counter_list.append(uppercase_counter) <br>
  case_counter_list.append(lowercase_counter) <br>
<br>
  return case_counter_list <br>

sentence = input() <br>
sentence = str(sentence) <br>
print('UPPER CASE', lowerUpperCase(sentence)[0] ) <br>
print('LOWER CASE', lowerUpperCase(sentence)[1] ) <br>

# Question 15

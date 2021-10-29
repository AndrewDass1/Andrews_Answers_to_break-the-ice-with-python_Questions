# Day 4 Solutions

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

# Question 15

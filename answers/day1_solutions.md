# Day 1 Solutions

# Question 1
```
for i in range(2000, 3201): <br>
  if i % 7 == 0 and i % 5 !=0 : <br>
    print(i, end=" ")
``` 
   
# Question 2
num = int(input("")) <br>
product_of_num = 1 <br>

while (num > 0): <br>
  product_of_num = product_of_num * num <br>
  num -= 1 <br>

print(product_of_num)

# Question 3
dictionary_of_num = {} <br>
num = int(input("")) <br>
num2 = 1 <br>

for i in range(1, num+1): <br>
  dictionary_of_num[num2] = num2**num2 <br>
  num2+=1 <br>

print(dictionary_of_num) 

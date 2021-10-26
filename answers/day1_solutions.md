# Day 1 Solutions

# Question 1
for i in range(2000, 3201):
  if i % 7 == 0 and i % 5 !=0 :
    print(i, end=" ")
    
# Question 2
num = int(input(""))
product_of_num = 1

while (num > 0):
  product_of_num = product_of_num * num
  num -= 1

print(product_of_num)

# Question 3
dictionary_of_num = {}
num = int(input(""))
num2 = 1

for i in range(1, num+1):
  dictionary_of_num[num2] = num2**num2
  num2+=1

print(dictionary_of_num) 

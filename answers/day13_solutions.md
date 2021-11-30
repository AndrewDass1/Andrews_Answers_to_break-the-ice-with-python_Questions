# Day 13 Solutions

# Question 47

# Q47 Task
Define a class named Circle which can be constructed by a radius. The Circle class has a method which can compute the area.
# Q47 Procedure
1. Make the class:
```
class Circle():
```
2. Make a method to create the radius and then another method to calcuate the circle area:
```
  def __init__(self, radius):
        self.radius = radius
        
    def area(self):
        self.radius = float(input(""))
        return self.radius**2*3.14
```
3. Test the class by assigning the class to a variable and then print it:
```
area_of_circle = Circle('')
print(area_of_circle.area())
```

# Q47 Solutions
```
class Circle():
    
    def __init__(self, radius):
        self.radius = radius
        
    def area(self):
        self.radius = float(input(""))
        return self.radius**2*3.14
    
area_of_circle = Circle('')
print(area_of_circle.area())
```

# Question 48

# Q48 Task
Define a class named Rectangle which can be constructed by a length and width. The Rectangle class has a method which can compute the area.

# Q48 Procedure
1. Create the rectangle class:
```
class Rectangle():
```
2. Create two static methods, one to initiate the rectangle's width and length and another method to calculate the rectangle area:
```
def __init__(self, width, length):
        self.width = width
        self.length = length
        
    def area(self):
        self.width = int(input(""))
        self.length = int(input(""))
        return self.width * self.length
```
3. Test the class by assigning the class to a variable and then print it:
```
rectangle_area = Rectangle('','')
print(rectangle_area.area())
```

# Q48 Solution
```
class Rectangle():
    
    def __init__(self, width, length):
        self.width = width
        self.length = length
        
    def area(self):
        self.width = int(input(""))
        self.length = int(input(""))
        return self.width * self.length
    
rectangle_area = Rectangle('','')
print(rectangle_area.area())
```

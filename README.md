#ulfa stevi juliana
#G1A022042
#Functional Programming (FP)
def square(num):
  return num ** 2

def map_square(numbers):
  return list(map(square, numbers))

numbers = [1, 2, 3, 4, 5]
squares = map_square(numbers)
print(squares)  #print : [1, 4, 9, 16, 25]


#Object-Oriented Programming (OOP)
class Rectangle:
  def __init__(self, width, height):
    self.width = width
    self.height = height

  def area(self):
    return self.width * self.height

rectangle = Rectangle(10, 5)
print(rectangle.area()) #print : 50


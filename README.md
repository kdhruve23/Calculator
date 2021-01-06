# Calculator

print("Use these Mathematical Operations keywords: add, sub, multiply, divide")
operation = input("Enter the mathematical operation you wish to conduct: ")

time = int(input("How many numbers do you wish to " + operation))
total = 0

#addition
if operation == 'add':
  for i in range(time):
    num = int(input("Enter digit: "))
    total += num

#subtraction
if operation == 'sub':
  for i in range(time):
    num = int(input("Enter digit: "))
    total -= num

#multiplication
if operation == 'multiply':
  num1 = int(input("Enter digit: "))
  total = num1
  for i in range(time-1):
    num = int(input("Enter digit: "))
    total = total * num

#division
if operation == 'divide':
  num1 = int(input("Enter digit: "))
  total = num1
  for i in range(time-1):
    num = int(input("Enter digit: "))
    total = total / num

print("Your solution is: " + str(total))

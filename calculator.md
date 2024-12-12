# satement 
it's a python calculator 

```python 
def calculater():
 try:
  # Get input from user

  operation = input("Enter operation (+, -, *, /):")

  if operation not in ["+", "-", "*", "/"]:
    raise ValueError("raise ValueError Invalid operation. Please enter one of +, -, *, /.")


  number1 = float(input("Enter first number:"))
  number2 = float(input("Enter second number:"))

  if operation == "+":
    result = number1 + number2
  elif operation == "-":
    result = number1 - number2
  elif operation == "*":
    result = number1 * number2
  elif operation == "/":
    result = number1 / number2
  else:
    result = "Invalid operation"

  print("The result is:", result)

 except ValueError as ve:
  print("Error", ve)



calculater()
```
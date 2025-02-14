## Python Function Challenge: Temperature Converter

Your task is to create a temperature conversion program using Python functions. This program will allow users to convert temperatures between Celsius and Fahrenheit scales.

**Requirements:**

1. Create two functions:
   - `celsius_to_fahrenheit(celsius)`: Converts Celsius to Fahrenheit
   - `fahrenheit_to_celsius(fahrenheit)`: Converts Fahrenheit to Celsius

2. Implement a main menu function that displays options and returns the user's choice.

3. Use a while loop to keep the program running until the user chooses to quit.

**Function Formulas:**
- Celsius to Fahrenheit: $$F = (C \times 9/5) + 32$$
- Fahrenheit to Celsius: $$C = (F - 32) \times 5/9$$

**Program Structure:**

```python
def celsius_to_fahrenheit(celsius):
    # Your code here

def fahrenheit_to_celsius(fahrenheit):
    # Your code here

def menu():
    # Your code here

def main():
    # Your code here

# Call the main function to start the program
main()
```

**Bonus Challenge:**
Add a third conversion option for Kelvin, including functions to convert to and from Kelvin.

## Submission:  Submit your code here and click "mark as done" on Google Classroom.
def celsius_to_fahrenheit(celsius):
  fahrenheit = (celsius * 9/5) + 32
  return fahrenheit

def fahrenheit_to_celsius(fahrenheit):
  celsius = (fahrenheit - 32) * 5/9
  return celsius

def kelvin_to_fahrenheit(kelvin):
  fahrenheit = (kelvin - 273.15) * 1.8 + 32
  return fahrenheit

def menu():
  while True:
    print("1. celsius to fahrenheit")
    print("2. fahrenheit to celsius")
    print("3. kelvin to fahrenheit")
    print("4. quit")
    choice = input("Pick a number 1, 2, 3, 4.")

    if choice == "1":
           celsius = eval(input("Enter celsius"))
           fahrenheit = celsius_to_fahrenheit(celsius)
           print(f"{celsius}°C = {fahrenheit:f}°F")
    if choice == "2":
           fahrenheit = eval(input("Enter Fahrenheit:"))
           celsius = fahrenheit_to_celsius(fahrenheit)
           print(f"{fahrenheit}°F = {celsius:f}°C")
    if choice == "3":
           kelvin = eval(input("Enter Kelvin"))
           fahrenheit = kelvin_to_fahrenheit(kelvin)
           print(f"{kelvin}°K = {fahrenheit: f}°F")
    if choice == "4":
      break
      

menu()

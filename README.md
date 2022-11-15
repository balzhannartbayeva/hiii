# hiii
How are you
 this example you will learn to create a simple calculator that can add, subtract, multiply or divide depending upon the input from the user.

To understand this example, you should have the knowledge of the following Python programming topics:

Python Functions
Python Function Arguments
Python User-defined Functions
Example: Simple Calculator by Using Functions
# Program make a simple calculator

# This function adds two numbers
def addition(x, z):
    return x + z

# This function subtracts two numbers
def subtraction(x, y):
    return x - y

# This function multiplies two numbers
def multiplication(x, y):
    return x * y

# This function divides two numbers
def division(x, y):
    return x / y


print("Select operation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")

while True:
    # take input from the user
    choice = input("Enter choice(1/2/3/4): ")

    # check if choice is one of the four options
    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
        
        # check if user wants another calculation
        # break the while loop if answer is no
        next_calculation = input("Let's do next calculation? (yes/no): ")
        if next_calculation == "no":
          break
    
    else:
        print("Invalid Input")

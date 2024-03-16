Project Documentation: Simple Calculator with Advanced Features

1. Introduction:
This project implements a simple calculator with advanced features using Python. The calculator can perform basic arithmetic operations such as addition, subtraction, multiplication, and division, along with exponentiation. Users have the option to select the desired operation or quit the calculator.

2. Features:

Addition: Adds two numbers.
Subtraction: Subtracts one number from another.
Multiplication: Multiplies two numbers.
Division: Divides one number by another (handles division by zero).
Exponentiation: Raises one number to the power of another.
Quit: Exits the calculator.
3. Code Explanation:

python
Copy code
# Define functions for basic arithmetic operations
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    else:
        return x / y

def exponentiate(x, y):
    return x ** y

# Main function to run the calculator
def calculator():
    print("Welcome to the Simple Calculator with Advanced Features!")
    print("Select operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exponentiation")
    print("6. Quit")

    while True:
        choice = input("Enter choice (1/2/3/4/5/6): ")

        if choice in ('1', '2', '3', '4', '5'):
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

            if choice == '1':
                print("Result:", add(num1, num2))
            elif choice == '2':
                print("Result:", subtract(num1, num2))
            elif choice == '3':
                print("Result:", multiply(num1, num2))
            elif choice == '4':
                print("Result:", divide(num1, num2))
            elif choice == '5':
                print("Result:", exponentiate(num1, num2))
        elif choice == '6':
            print("Thank you for using the calculator. Goodbye!")
            break
        else:
            print("Invalid input. Please enter a valid option.")

# Entry point of the program
if __name__ == "__main__":
    calculator()
4. Execution:

When the program is run, it displays a welcome message and prompts the user to select an operation.
The user inputs the desired operation (1-6).
Based on the user's choice, the calculator prompts for two numbers and performs the selected operation.
The result is displayed, and the user can continue with another operation or quit.
5. User Interaction:


6. Conclusion:
This Python program provides a simple yet functional calculator with advanced features. It demonstrates basic arithmetic operations and incorporates user-friendly interaction for seamless use.

7. Future Improvements:

Error handling for invalid inputs.
Support for more advanced mathematical functions.
Graphical user interface (GUI) implementation for better user experience.# CODETECHPYTASK

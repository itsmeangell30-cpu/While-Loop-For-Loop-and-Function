# While-Loop-For-Loop-and-Function
Python programs demonstrating loops (while and for) and functions through practical examples like a Number Guessing Game, Multiplication Table Generator, and BMI Calculator. Practice control statements, iteration, function creation, and basic problem-solving using Python.

 Python Programming: While Loop, For Loop & Functions
!Python !Level !Status !Learning

📌 Project Overview
🔹 This repository contains three beginner-friendly Python programs demonstrating loops, control statements, and functions.

🔹 Each program focuses on a fundamental programming concept through a practical example.

🔹 The project helps improve logical thinking, problem-solving, and coding skills.

🎯 Objectives
🟢 Understand while loops and loop control statements.
🔵 Practice for loops using the range() function.
🟣 Learn how to define and call Python functions.
🟡 Accept user input and display calculated results.
🟠 Apply Python concepts to simple real-world problems.

🎮 Program 1: Number Guessing Game

📖 Description
Uses a while loop to create an interactive number guessing game.
Generates a random number between 1 and 10 using the random module.
Allows the user three valid guesses.
Provides feedback when the guess is too high or too low.
Uses continue to skip invalid out-of-range guesses.
Uses break to stop the loop when the correct number is guessed.
Uses the while loop's else clause to display a message when attempts run out.

💻 Python Code
import random

secret_number = random.randint(1, 10)
attempts = 3

while attempts > 0:
    guess = int(input("Guess the number (between 1 and 10): "))

    if guess < 1 or guess > 10:
        print("Your guess is out of range. Please guess a number between 1 and 10.")
        continue

    attempts -= 1

    if guess == secret_number:
        print("Congratulations! You guessed the correct number.")
        break
    elif guess > secret_number:
        print("Too high. Try again.")
    else:
        print("Too low. Try again.")

else:
    print("Better luck next time! The correct number was", secret_number)

🖥️ Sample Output
Guess the number (between 1 and 10): 2
Too low. Try again.
Guess the number (between 1 and 10): 15
Your guess is out of range. Please guess a number between 1 and 10.
Guess the number (between 1 and 10): 5
Too high. Try again.
Guess the number (between 1 and 10): 3
Congratulations! You guessed the correct number.

🧠 Concepts Learned
🔹 while loop
🔹 if, elif, and else
🔹 break and continue
🔹 Random number generation
🔹 User input and conditional logic

🔢 Program 2: Multiplication Table Generator

📖 Description
Generates a multiplication table for a number entered by the user.
Uses a for loop to iterate from 1 to 10.
Uses range(1, 11) to repeat the loop ten times.
Calculates the product of the entered number and each loop value.
Displays the multiplication table in a clear, readable format.

💻 Python Code
number = int(input("Enter the number for which you want the multiplication table: "))

for i in range(1, 11):
    result = number * i
    print(number, "x", i, "=", result)

🖥️ Sample Output
Enter the number for which you want the multiplication table: 5
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50

🧠 Concepts Learned
🔹 for loop
🔹 range() function
🔹 Arithmetic operators
🔹 Variables and user input
🔹 Formatted output

⚖️ Program 3: BMI Calculator Using Functions
📖 Description
Calculates Body Mass Index (BMI) using a user-defined Python function.
Accepts the user's weight in kilograms and height in meters.
Uses the BMI formula to calculate the result.
Returns the calculated value from the function.
Displays the BMI rounded to two decimal places.

📐 Formula
BMI = Weight (kg) / Height (m)²

💻 Python Code
def calculate_bmi(weight, height):
    bmi = weight / (height ** 2)
    return bmi

weight = float(input("Enter your weight in kg: "))
height = float(input("Enter your height in meters: "))

bmi = calculate_bmi(weight, height)

print("Your BMI is:", format(bmi, ".2f"))
🖥️ Sample Output
Enter your weight in kg: 58
Enter your height in meters: 1.62
Your BMI is: 22.10
🧠 Concepts Learned
🔹 Defining functions with def
🔹 Function parameters and arguments
🔹 Returning values with return
🔹 Floating-point input using float()
🔹 Mathematical calculations and exponentiation
🔹 Formatting decimal output
🛠️ Technologies Used
🐍 Python 3
📓 Jupyter Notebook or any Python IDE

🚀 How to Run the Programs
Install Python 3 on your computer.
Open Jupyter Notebook, VS Code, or another Python environment.
Create a Python file or notebook cell for each program.
Copy the corresponding code into the editor.
Run the program and enter the requested input.
Observe the output and experiment with different values.


🌟 Key Learning Outcomes
🟢 Understand how loops repeat instructions.
🔵 Control loop execution using break and continue.
🟣 Generate sequences using range().
🟡 Organize reusable logic using functions.
🟠 Perform calculations using user-provided data.
🔴 Improve debugging, logical thinking, and problem-solving skills.

📸 Visual Highlights
🎮 Number Guessing Game	🔢 Multiplication Table	⚖️ BMI Calculator
Random number generation	Repeated multiplication	BMI calculation
while loop	for loop	User-defined function
break and continue	range()	return statement

👩‍💻 Who Is This Project For?
🌱 Python beginners
📚 Students completing Python assignments
💡 Learners practicing loops and functions
🧩 Anyone building a foundation in programming

💻 Keep learning, keep coding, and keep growing with Python!

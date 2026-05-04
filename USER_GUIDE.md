# User Guide
Hello and welcome to my grade calculator. This is a C++ console application that tracks graded items (homework, quizzes, exams) and calculates points-based and weighted final grades, built around an inheritance hierarchy with a menu-driven interface.

## How to get started:
- Using g++ (Linux / macOS / WSL / MinGW): g++ -std=c++17 *.cpp -o GradeCalculator

## The features:
- Set Grading Scheme - Allows you to make a custom grading scheme to better your school's grading system. You will be asked to input 3 floats that add up to EXACTLY 100.0 for the weights of each of the 3 assignment types (homework, quiz, and exam), then 4 more floats to determine each of the cutoffs.
- Add Graded Item - Creates a GradedItem object to store in a vector of assignments. You will be asked to select what category of assignment you want to add from homework, quiz and exam, the name of the assignemnt, the amount of points you got for that assignment and how many points you could have earned.
- Edit Item - Allows you to edit an item in the vector of assignments. You will be asked to provide the index of the assignment you wish to edit, the specific thing you which to change about it, and what to change it to.
- View All Items - Shows all assignments you have entered. You don't need to provide any additional input upon selecting this option.
- Remove Item - Removes an item of your choice from the vector of assignments. You will provide the index of the assignment you want to remove, then provide confirmation for removing said assignment.
- Calculate Grade (Points-based) - Calculates your grade, treating all assignments as having the same weight. No additional input should be required.
- Calculate Grade (Weighted) - Calulates your grade using your grading scheme's weights. No additional input should be required, there's a preset grading scheme in place should you not have run the Set Grading Scheme Function prior to calling this.
- Exit - Enough said.

## Sprint Additions:
- Lab 19 - Rejecting non-numeric inputs without the program crashing via cin.fail(). a program that crashes on bad input isn't too reliable now, is it?
- Lab 20 - A function to edit items in the vector of assignments. This one has already been mentioned above.
- Lab 21 - ASNI colors for letter grades and the menu interface to help it feel less bland and give it a better first impression.
- Lab 22 - Confirmation for deleting an object after it's been selected. It's not much, but it does do a lot.

## The difference between points-based and weighted grade modes:
- Points-based grading sums up the total points you earned on all of your assignments, then divides that by the total amount of points you could have earned from all assignments to get your percentage.
- Weighted grading sums up the average of each category individually, then multiplies them by their respective weights before adding them together to get your final grade.

## Known limitations:
- The grade calculator wasn't made to handle extra credit or bonus points.
- You cannot save assignments. You will have to manually add each assignment to the calculator every time you use it.
- This isn't the most efficient calculator by any means, but it works and doesn't crash on bad input.

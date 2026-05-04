# User Guide
Hello and welcome to my grade calculator. This is a C++ console application that tracks graded items (homework, quizzes, exams) and calculates points-based and weighted final grades, built around an inheritance hierarchy with a menu-driven interface.

## How to get started:
- Using g++ (Linux / macOS / WSL / MinGW): g++ -std=c++17 *.cpp -o GradeCalculator

## The features:
- Set Grading Scheme - Allows you to make a custom grading scheme to better your school's grading system. You will be asked to input 3 floats that add up to EXACTLY 100.0 for the weights of each of the 3 assignment types (homework, quiz, and exam), then 4 more floats to determine each of the cutoffs.
- Add Graded Item - Creates a GradedItem object to store in a vector of assignments. You will be asked to select what category of assignment you want your
- Edit Item -
- View All Items - Shows all assignments you have entered. You don't need to provide any additional input upon selecting this option.
- Remove Item - Removes an item of your choice from the vector of assignments. You will provide the index of the assignment you want to remove, then provide confirmation for removing said assignment.
- Calculate Grade (Points-based) - Calculates your grade, treating all assignments as having the same weight. No additional input should be required.
- Calculate Grade (Weighted) - Calulates your grade using your grading scheme's weights. No additional input should be required, there's a preset grading scheme in place should you not have run the Set Grading Scheme Function prior to calling this.
- Exit - Enough said.


## Known limitations:
- The grade calculator wasn't made to handle extra credit or bonus points.
- You cannot save assignments. You will have to manually add each assignment to the calculator every time you use it.
- This isn't the most efficient calculator by any means, but it works and doesn't crash on bad input.

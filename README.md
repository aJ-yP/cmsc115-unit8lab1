# Lab Reflection: Unit 8 Lab 1 - Git Version Control + Debugging (BuggyProgram)

## Student Name
Artries John Pangilinan

## GitHub Repository URL
https://github.com/aJ-yP/cmsc115-unit8lab1.git

---

# Commit 1: Initial Commit

## What did you include in this commit?
- I included the original BuggyProgram.java file, the three JUnit test classes, and the
- README.md file.

## What was the purpose of this commit?
- The purpose was to save the original project before making any changes. This established a
- baseline that I could use to compare my fixes and track my progress though git.

---

# Commit 2: Task 1 (getGrade)

## Which tests in Task1Test were failing before your fix?
- The tests checking the grade categories and score boundaries were failing because the method 
- returned the wrong category for certain scores.

## What was the issue in the code?
- The conditional statements used incorrect comparison operators and returned the wrong 
- performance categories. The original code also assigned "Meets" to scores above 90 instead 
- of "Exceeds".

## What change did you make to fix it?
- I corrected the order of the grade categories and changed the comparison operators to include
- the boundary values. Scores of 90 or higher return "Exceed", scores of 80 or higher but below
- 90 return "Meets", and scores below 80 return "Does Not Meet".

## How did the tests help guide your fix?
- The tests showed the expected and actual results,which helped me identify the incorrect
- category assignments and boundary conditions.

---

# Commit 3: Task 2 (sumEvenNumbers)

## Which tests in Task2Test were failing before your fix?
- The tests checking the sum of even numbers were expected to fail because the original method
- initialized the sum incorrectly and used an invalid loop boundary.

## What was the issue in the code?
- The sum started at 1 instead of 0, which caused incorrect totals. The loop also used
- i <= values.length, allowing it to access an array index outside the valid range.

## What change did you make to fix it?
- I initialized the sum to 0 and changed the loop condition to i < values.length. This allows
- the method to examine every valid array element without going beyond the array's bounds.

## How did the tests help guide your fix?
- The tests helped expose the array boundary problem.

---

# Commit 4: Task 3 (sumRange)

## Which tests in Task3Test were failing before your fix?
-

## What was the issue in the code?
-

## What change did you make to fix it?
-

## How did the tests help guide your fix?
-

---

# Overall Reflection

## Which task was the easiest to fix? Why?
-

## Which task was the most difficult? Why?
-

## How did Git help you track your progress through the debugging process?
-

## Why is it important to make small, frequent commits when debugging code?
-

## What did you learn about using JUnit tests to guide debugging?
-

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
-

## Why is it useful to document your work after completing a programming task?
-
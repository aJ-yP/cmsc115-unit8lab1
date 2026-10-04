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
- The test for sumRange(5, 0) was failing because the method returned 0 instead of 15.

## What was the issue in the code?
- The original loop only counted upward from the starting number to the ending number. When
- the starting number was greater than the ending number, the loop condition was false
- immediately, so the loop never executed.

## What change did you make to fix it?
- I added an if and else statement with two for loops. The first loop counts upward when the
- starting number is less than or equal to the ending number. The second loop counts downward
- when the starting number is greater than the ending number.

## How did the tests help guide your fix?
- The tests helped me identify that the method worked for ranges that counted upward but failed
- for ranges that counted downward.

---

# Overall Reflection

## Which task was the easiest to fix? Why?
- Task 2 was relatively easy to understand because the problems were clear in the code. The
- incorrect starting value and loop boundary explained why the method could cause an array index
- error.

## Which task was the most difficult? Why?
- Task 3 was the most difficult because I had to figure out how to make the method work when
- the starting number was greater than the ending number. The original loop only counted
- upward, so it did not work for descending ranges.

## How did Git help you track your progress through the debugging process?
- Git allowed me to save each stage of my work in separate commits. This made it easier to track
- the changes for each task, and review my progress.

## Why is it important to make small, frequent commits when debugging code?
- Small, frequent commits keep changes organized and make it easier to identify which
- modification cause a problem r fixed a bug. They also make it easier to review the project
- history and undo a specific change without losing unrelated work.

## What did you learn about using JUnit tests to guide debugging?
- I learned that JUnit tests can reveal logical errors that may not be obvious from reading
- the code alone. Comparing expected and actual results helps narrow down the source of the
- problem. Rerunning tests after making changes also helps verify that the fix works
- as intended.

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
- Before making the final commit, I completed the debugging tasks, updated the README with
- my reflections, checked project files, and verified that the JUnit tests passed. I also
- confirmed that my changes were committed and pushed to GitHub.

## Why is it useful to document your work after completing a programming task?
- Documenting my work helps explain the problems I encountered, the changes I made, and how
- I verified the results. It also makes the project easier for other developers to understand
- and maintain. Recording the debugging process gives me something to reference when I encounter
- similar problems in the future.
🔢 NumPy Analyzer
A Menu-Driven Array Operations and Statistics Project in Python
Project: NumPy Analyzer
Programming Language: Python 3
Core Library: NumPy
Application Type: Command-Line Interface (CLI)
Purpose: Educational project demonstrating numerical array
operations

📌 1. Project Overview
NumPy Analyzer is a menu-driven Python application developed to
demonstrate the use of the NumPy library for numerical computing. It
allows users to create arrays, perform element-wise mathematical
operations, combine or split arrays, search and sort values, filter
data, and calculate basic statistical measures.

The program presents a main menu and asks the user to select an
operation. It is a practical project for learning how NumPy makes
numerical operations easier and more efficient.
🎯 2. Project Objectives
The main objectives of this project are to:
- Learn how to create one-dimensional (1D), two-dimensional (2D), and
  three-dimensional (3D) NumPy arrays.
- Perform addition, subtraction, multiplication, and division on
  arrays.
- Understand array indexing and slicing.
- Combine and split arrays.
- Search for values and sort array elements.
- Filter values using a condition.
- Calculate sum, mean, median, standard deviation, and variance.
- Practise Python loops, conditional statements, user input, and
  menu-driven programming.
✨ 3. Features
  Feature                             Description
  🧱 Create Arrays                    Create 1D, 2D, and 3D arrays using
                                      user input.

  📍 Indexing                         Access an element by its index.

  ✂️ Slicing                          Select a section of a 2D array
                                      using row and column ranges.

  ➕ Mathematical Operations          Perform addition, subtraction,
                                      multiplication, and division
                                      element by element.

  🔗 Combine Arrays                   Combine compatible 2D arrays
                                      vertically with np.vstack().

  🧩 Split Arrays                     Split a 2D array vertically using
                                      np.vsplit().

  🔎 Search                           Find the indices of a specified
                                      value with np.where().

  🔢 Sort                             Sort array values using
                                      np.sort().

  🎯 Filter                           Display values greater than a
                                      selected threshold.

  📊 Statistics                       Calculate sum, mean, median,
                                      standard deviation, and variance.

  🚪 Exit                             Exit the program using the main
                                  menu.
🛠️ 4. Technologies and Requirements
- Python 3: Main programming language.
- NumPy: Numerical library used for array creation and
  calculations.
- Terminal / Command Prompt: Used to run the program and provide
  input.
Prerequisites
- Python 3 installed on the computer.
- NumPy installed in the same Python environment used to run the
  program.
- Basic understanding of Python input, loops, and conditions.
📥 5. Installation and Execution
Step 1: Install Python
Download Python from the official website:

https://www.python.org/downloads/

On Windows, select Add Python to PATH during installation if the
option is available.
Step 2: Install NumPy
Open Command Prompt or a terminal and execute:
python -m pip install numpy
If you use the Windows Python launcher, you can try:
py -m pip install numpy
Step 3: Save the Python File
Save the project code in a file named:
numpy_analyzer.py
Step 4: Run the Program
Open a terminal in the folder containing the file and run:
python numpy_analyzer.py
On Windows, this alternative may also work:
py numpy_analyzer.py
🧭 6. Main Menu
The program displays this menu when it starts:
Welcome to the NumPy Analyzer!
=======================================
Main Menu - Choose an option:
1. Create a NumPy Array
2. Perform Mathematical Operations
3. Combine or Split Arrays
4. Search, Sort, or Filter Arrays
5. Compute Aggregates and Statistics
6. Exit
Enter your choice:
Menu Description
1. Create a NumPy Array: Create a 1D, 2D, or 3D array and access
   indexing or slicing options.
2. Perform Mathematical Operations: Perform arithmetic operations
   on compatible arrays.
3. Combine or Split Arrays: Vertically combine two arrays or split
   an existing 2D array.
4. Search, Sort, or Filter Arrays: Find values, sort the array, or
   display values above a threshold.
5. Compute Aggregates and Statistics: Calculate sum, mean, median,
   standard deviation, or variance.
6. Exit: End the program.
🧪 7. Sample Operations and Expected Results
The following examples demonstrate the intended behavior of the NumPy
operations.
Example 1: Create a 1D Array
Input elements:
10 20 30 40
Expected array:
[10 20 30 40]
Example 2: Add Two 2D Arrays
First array:
[[1 2]
 [3 4]]
Second array:
[[5 6]
 [7 8]]
Expected addition result:
[[ 6  8]
 [10 12]]
NumPy performs the operation element by element because the arrays have
the same shape.
Example 3: Search for a Value
Given the array:
[[10 20]
 [30 20]]
Search for the value 20.

Using zero-based indexing, it occurs at:
- Row 0, column 1
- Row 1, column 1
np.where() returns the matching index positions.
Example 4: Filter Values
Given the array:
[[10 20]
 [30 40]]
For a threshold of 20, the expression:
arr1[arr1 > 20]
returns:
[30 40]
The value 20 is excluded because the condition is strictly greater
than 20.
Example 5: Calculate Statistics
For the values [10, 20, 30, 40]:

  Statistical Operation         Expected Result
  Sum                                       100
  Mean                                     25.0
  Median                                   25.0
  Standard Deviation        Approximately 11.18
  Variance                                125.0

NumPy uses population standard deviation and population variance by
default (ddof=0).
🧠 8. NumPy Functions and Concepts Used
  Function / Concept                  Purpose
  np.array()                        Converts input values into a NumPy
                                      array.

  .reshape()                        Changes an array's shape when the
                                      number of elements is compatible.

  np.vstack()                       Stacks arrays vertically when their
                                      column dimensions match.

  np.vsplit()                       Splits an array vertically into
                                      sections.

  np.where()                        Finds indices where a condition is
                                      true.

  np.sort()                         Returns a sorted copy of an array.

  np.sum()                          Calculates the sum of array
                                      elements.

  np.mean()                         Calculates the arithmetic mean.

  np.median()                       Calculates the median value.

  np.std()                          Calculates standard deviation.

  np.var()                          Calculates variance.

  Boolean indexing                    Selects array elements that satisfy
                                      a condition.

  np.any()                          Checks whether at least one element
                                      satisfies a condition.

  while True                        Repeats the main menu until the
                                      program exits.

  if / elif / else                  Selects which operation to execute.

  break                             Ends the menu loop when Exit is
                                  selected.
⚙️ 9. Program Workflow
1. Import the library: import numpy as np loads NumPy and assigns
   it the short alias np.
2. Display the welcome message: The program introduces the NumPy
   Analyzer.
3. Show the main menu: A while True loop keeps displaying the
   options.
4. Read the selection: input() collects the user's choice, and
   int() converts it to an integer.
5. Select the operation: Conditional statements route the program
   to the selected menu branch.
6. Create or process arrays: User-entered numbers are converted
   into arrays. .reshape() arranges elements into the requested
   dimensions.
7. Calculate and display results: The selected NumPy function
   performs the requested operation, and print() displays the result.
8. Exit: Choosing option 6 executes break and stops the loop.
⚠️ 10. Current Version: Important Limitations
This README describes the behavior and limitations of the supplied
source code. The following issues should be addressed before a final
demonstration:
- Array initialization: Options 2--5 use arr1, but it is created
  only when the user creates a 2D array. Selecting those options first
  can cause a NameError.
- 1D and 3D indexing: The indexing submenu always asks for row and
  column indices, which does not correctly handle all array
  dimensions.
- Slicing: The current slicing code reshapes elements using
  rows and cols. Those variables may be undefined or may not match
  the most recently created array.
- Mathematical operations: The second array must have the same
  shape as the first array for the intended element-wise results. The
  code does not validate the number of entered elements before
  reshaping.
- Combining arrays: np.vstack() requires the arrays to have
  matching column dimensions.
- Splitting arrays: The requested number of vertical splits must
  be valid for the array's row count.
- Invalid input: Entering letters instead of numbers can cause
  ValueError. Invalid dimensions and index ranges also need
  validation.
- Input consistency: The program should store the active array
  consistently so that each menu option operates on the intended data.
These are known limitations of the supplied version, not features that
have already been fixed. Correcting them and testing all menu options
will improve reliability and presentation quality.
🚀 11. Future Enhancements
Potential improvements include:
- Add input validation and friendly error messages.
- Maintain a single active array or clearly manage separate arrays.
- Support indexing and slicing correctly for 1D, 2D, and 3D arrays.
- Validate array dimensions and element counts before reshaping.
- Add horizontal stacking and other array-combination options.
- Add minimum, maximum, and additional statistical calculations.
- Create automated tests for valid and invalid inputs.
- Develop a graphical user interface (GUI).
🎓 12. Learning Outcomes
After developing and studying this project, a student can demonstrate an
understanding of:
- Python loops and conditional statements.
- Taking input and converting data types.
- Creating and reshaping NumPy arrays.
- Performing element-wise mathematical calculations.
- Searching, sorting, and filtering array data.
- Combining and splitting compatible arrays.
- Calculating basic statistical measures.
- Identifying program errors and documenting limitations.
🏁 13. Conclusion
NumPy Analyzer is an educational project that brings essential NumPy
operations together in a single menu-driven Python application. It
demonstrates how arrays can be created, processed, searched,
reorganized, and analyzed using numerical and statistical functions.

The project provides a foundation for learning Python-based numerical
computing. With input validation, consistent array management,
dimension-aware indexing, and systematic testing, it can become a more
reliable and complete application.
👨‍💻 Project Details
- Project Name: NumPy Analyzer
- Language: Python 3
- Library: NumPy
- Interface: Command-Line Interface (CLI)
- Project Category: Educational / Numerical Computing
Student Details
- Student Name: \(Enter your name\)
- Class / Course: \(Enter your class or course\)
- Roll Number: \(Enter your roll number\)
- Institution: \(Enter your college or school name\)
- Submitted To: \(Enter your teacher's name\)
Prepared for academic submission and project demonstration.

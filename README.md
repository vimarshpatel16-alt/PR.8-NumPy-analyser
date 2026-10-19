🔢 NumPy Analyzer
A Menu-Driven Python Project for Array Operations and Statistical Analysis
<p align="center">
<strong>{=html}Explore NumPy arrays, mathematical operations, array
manipulation, searching, filtering, and statistics through an
interactive command-line menu.</strong>{=html}
</p>
📌 Project Information
  Item                   Details
  Project Name           NumPy Analyzer
  Programming Language   Python 3
  Main Library           NumPy
  Interface              Command-Line Interface (CLI)
  Project Type           Educational Python Project
📖 1. Introduction
NumPy Analyzer is a menu-driven Python application that demonstrates
fundamental numerical computing operations using the NumPy library. It
allows users to create arrays, perform arithmetic calculations, combine
or split arrays, search and sort values, filter data, and calculate
statistical measurements.

The application displays a main menu and lets the user select an
operation. This project provides hands-on practice with NumPy and
important Python programming concepts.
🎯 2. Project Objectives
The objectives of this project are to:
- Understand NumPy and its role in numerical computing.
- Create one-dimensional (1D), two-dimensional (2D), and
  three-dimensional (3D) arrays.
- Perform element-wise addition, subtraction, multiplication, and
  division.
- Practise array indexing and slicing.
- Combine and split compatible arrays.
- Search for values, sort elements, and filter data using conditions.
- Calculate sum, mean, median, standard deviation, and variance.
- Apply Python loops, conditional statements, user input, and
  menu-driven programming.
✨ 3. Main Features
  Feature                             Description
  🧱 Array Creation                   Create 1D, 2D, and 3D arrays from
                                      user-provided integers.

  📍 Indexing                         Access an element using its index.

  ✂️ Slicing                          Select a range of rows and columns
                                      in a 2D array.

  ➕ Arithmetic Operations            Perform addition, subtraction,
                                      multiplication, and division
                                      element by element.

  🔗 Combine Arrays                   Stack compatible 2D arrays
                                      vertically using np.vstack().

  🧩 Split Arrays                     Split a 2D array vertically using
                                      np.vsplit().

  🔎 Search                           Locate matching values using
                                      np.where().

  🔢 Sort                             Sort array elements using
                                      np.sort().

  🎯 Filter                           Select values greater than a
                                      specified threshold.

  📊 Statistics                       Calculate sum, mean, median,
                                      standard deviation, and variance.

  🚪 Exit                             Exit the application from the main
                                  menu.
🛠️ 4. Technologies Used
- Python 3: Core programming language.
- NumPy: Library for numerical arrays and mathematical operations.
- Command Prompt / Terminal: Runs the application and accepts user
  input.
- Text Editor or IDE: For example, IDLE, VS Code, or PyCharm.
📥 5. Installation and Setup
Prerequisites
- Python 3 must be installed.
- NumPy must be installed in the Python environment used to run the
  project.
Step 1 --- Install Python
Download Python from the official website:

https://www.python.org/downloads/

On Windows, select Add Python to PATH during installation if that
option is shown.
Step 2 --- Install NumPy
Open Command Prompt or a terminal and run:
python -m pip install numpy
If you use the Windows Python launcher, try:
py -m pip install numpy
Step 3 --- Save the Code
Save the project source code as:
numpy_analyzer.py
Step 4 --- Run the Project
Open a terminal in the directory containing the file and run:
python numpy_analyzer.py
On Windows, this may also work:
py numpy_analyzer.py
🧭 6. Application Menu
When the program starts, it displays the following menu:
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
Menu Options Explained
1. Create a NumPy Array - Select a 1D, 2D, or 3D array. - Enter
integer elements. - Choose an indexing, slicing, or return option.

2. Perform Mathematical Operations - Select addition, subtraction,
multiplication, or division. - Enter the elements of a second array. -
View the element-wise result.

3. Combine or Split Arrays - Combine compatible 2D arrays
vertically. - Split a 2D array into vertical sections.

4. Search, Sort, or Filter Arrays - Search for a particular value. -
Sort array elements. - Display elements greater than a threshold.

5. Compute Aggregates and Statistics - Calculate the sum, mean,
median, standard deviation, or variance.

6. Exit - Display a thank-you message and end the program.
🧪 7. Sample Inputs and Expected Results
The examples below demonstrate the intended NumPy operations. They are
illustrative examples, not screenshots or logs captured from a program
run.
Example A --- Create a 1D Array
Input elements:
10 20 30 40
Expected array:
[10 20 30 40]
Example B --- Add Two 2D Arrays
First array:
[[1 2]
 [3 4]]
Second array:
[[5 6]
 [7 8]]
Expected addition result:
[[ 6  8]
 [10 12]]
NumPy performs element-wise addition when the arrays have compatible
shapes.
Example C --- Search for a Value
Given:
[[10 20]
 [30 20]]
Searching for 20 finds these zero-based positions:
- Row 0, column 1
- Row 1, column 1
The np.where() function returns the matching index coordinates.
Example D --- Filter Values
Given:
[[10 20]
 [30 40]]
With a threshold of 20, the expression:
arr1[arr1 > 20]
returns:
[30 40]
The value 20 is excluded because the condition is strictly greater
than 20.
Example E --- Calculate Statistics
For the values [10, 20, 30, 40]:

  Operation                  Expected Result
  Sum                                    100
  Mean                                  25.0
  Median                                25.0
  Standard Deviation     Approximately 11.18
  Variance                             125.0

Note: np.std() and np.var() use population formulas by default
(ddof=0).
🧠 8. NumPy Functions Used
  Function / Concept                  Explanation
  np.array()                        Creates a NumPy array from input
                                      values.

  .reshape()                        Changes array dimensions when the
                                      element count matches the requested
                                      shape.

  np.vstack()                       Stacks arrays vertically when their
                                      column dimensions match.

  np.vsplit()                       Splits an array vertically into
                                      sections.

  np.where()                        Returns indices where a condition
                                      is true.

  np.sort()                         Returns a sorted copy of the array.

  np.sum()                          Calculates the sum of elements.

  np.mean()                         Calculates the arithmetic average.

  np.median()                       Calculates the median.

  np.std()                          Calculates standard deviation.

  np.var()                          Calculates variance.

  np.any()                          Checks whether at least one element
                                      meets a condition; used here to
                                      detect zeros before division.

  Boolean indexing                    Selects elements that satisfy a
                                  condition.
⚙️ 9. Program Logic and Workflow
1. Import NumPy: import numpy as np imports the library using the
   alias np.
2. Display the welcome message: The application prints its title.
3. Repeat the main menu: while True keeps the menu running.
4. Read the user's choice: input() collects the choice, and
   int() converts it to an integer.
5. Choose a branch: if, elif, and else statements select the
   requested feature.
6. Create arrays: Input numbers are converted into NumPy arrays.
   .reshape() creates the requested 2D or 3D shape.
7. Perform operations: NumPy functions carry out calculations,
   search, sorting, filtering, or array manipulation.
8. Show results: print() displays the output.
9. Exit: Selecting option 6 executes break, stopping the menu
   loop.
⚠️ 10. Known Limitations of the Supplied Code
The following issues exist in the supplied version and should be
corrected before a final project demonstration:
- Array initialization: Options 2--5 use arr1, but it is only
  assigned in the 2D-array creation branch. Selecting those options
  before creating a 2D array may raise a NameError.
- Indexing: The indexing submenu always asks for row and column
  indices. This does not correctly support every 1D, 2D, or 3D array.
- Slicing: The code rebuilds an array using rows and cols,
  which may be undefined or inconsistent with the current array.
- Shape validation: The program does not verify that the user
  entered the exact number of elements required before calling
  .reshape().
- Array compatibility: Element-wise mathematical operations
  require compatible shapes. Vertical stacking also requires matching
  column counts.
- Splitting: The number of vertical splits must be valid for the
  number of rows.
- Invalid input: Entering non-numeric menu input may raise
  ValueError; index and dimension errors are not fully handled.
- Array consistency: A single, consistently managed active array
  would make it clearer which data each menu option uses.
These are limitations of the current source code. They are not claimed
to be fixed in this documentation. Fixing them and testing each menu
option will improve the project's reliability.
🚀 11. Future Enhancements
Possible future improvements include:
- Add validation for menu choices, dimensions, and array element
  counts.
- Handle errors with clear, user-friendly messages.
- Maintain a consistent active array across menu operations.
- Implement dimension-aware indexing and slicing for 1D, 2D, and 3D
  arrays.
- Add horizontal stacking and more array manipulation features.
- Include minimum, maximum, and additional descriptive statistics.
- Add automated tests for valid and invalid inputs.
- Develop a graphical user interface (GUI).
🎓 12. Learning Outcomes
Through this project, students can practise and demonstrate:
- Python variables, loops, conditions, and user input.
- Creating and reshaping NumPy arrays.
- Performing element-wise numerical calculations.
- Searching, sorting, and filtering array data.
- Combining and splitting compatible arrays.
- Calculating basic statistical measures.
- Identifying bugs and documenting software limitations.
- Organizing a Python program into clear menu-driven features.
🏁 13. Conclusion
NumPy Analyzer is an educational Python project that brings
essential NumPy array operations into one menu-driven application. It
demonstrates how numerical data can be created, manipulated, searched,
filtered, and analyzed using NumPy functions.

The project provides a foundation for learning numerical computing in
Python. Adding stronger input validation, consistent array management,
dimension-aware indexing, and systematic testing would make it more
robust and presentation-ready.

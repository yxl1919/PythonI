Week zero Help Center
 
Comments — CodeSkulptor
Non-computational parts of the program that textually describe the behavior of the program.
Comments begin with #, everything to right of the hash is ignored by Python.
Comments should be frequent so you and others can understand the code.
Lecture examples - CodeSkulptor
More examples - Comments, Strings, and Print
Strings — CodeSkulptor 
Sequence of characters enclosed by a pair of single or double quotes
Examples are "cats hate dogs" and 'Strings are fun!'.
Strings are one kind of data in Python. Their data type is denoted str.
Lecture examples - Hello World
More examples - Comments, Strings, and Print 
Numbers — Arithmetic Expressions
There are two kinds of numerical data in Python: integers and decimal numbers.
Integers correspond to the data type int. Decimal numbers are represented by floating-point numbers corresponding to the data type float.
Floating-point numbers have around 15 decimal digits of accuracy.
In CodeSkulptor, all numbers (even integers) are represented internally as floating-point numbers.
Lecture examples - Arithmetic Expressions 
More examples - Floats and Ints
Arithmetic Operators — Arithmetic Expressions
Five basic arithmetic operators; addition (+), subtraction (-), multiplication (*), division (/) and exponentiation (**)
CodeSkulptor implements a subset of Python 2. In Python 2, the division operator (/) returns a float approximation to the exact answer if either of the operands is a  float.  If both operands are integers, division returns the exact answer round down to the nearest integer.
The integer division operator // returns the quotient of two numbers..
Lecture examples - Arithmetic Expressions
More examples - Arithmetic Operations, Division
Arithmetic Expressions — Arithmetic Expressions
An arithmetic expression is either a number or an operator applied to two arithmetic expressions.
Arithmetic expressions are entered as a sequence of numbers and arithmetic operators.
Expressions are formed by grouping operators and operands via precedence: "Please excuse my dear Aunt Sallie"; parentheses, exponentiation, multiplication, division, addition, subtraction.
Lecture examples - Arithmetic Expressions
More examples - Order of Operations for Arithmetic Expressions, Possible Errors for Arithmetic Expressions
Variables — Variables
Variable names consist of a sequence of letters, number and underscores (_).
Variable names start with a letter or underscore and are case sensitive.
Single equals (=) is used for assignment to variables. Double equals (==) is used for testing equality.
Lecture examples - Variables
More examples - Variable Naming, Vabiable Assignment, Variable Operations, Formulas



Week one Help Center

Functions — Functions
Functions are reusable pieces of programs that take an input and produce an output.
A function definition is a compound statement consisting of a header and a body.
The header includes the keyword def, a sequence of parameters enclosed by parentheses, followed by a colon :.
The body consists of a sequence of statements, all indented by 4 spaces.
Functions may return a value using the keyword return or have a side effect (e.g., print).
To evaluate a function call, replace the function's parameters in the body of the function by their associated values in the call and execute the body of the function.
Lecture examples - Functions
More examples - Stucture of Functions, Uses of Functions, Scope of Variables, Examples of Functions
Indentation — Functions
Indentation consists of whitespace formed by blanks, tabs, and newlines.
Leading white space indicates indentation level (4 spaces per level) and specifies logical grouping of statements in Python.
Incorrect indentation can lead to errors.
Lecture examples - Functions
More examples - Function Errors
Remainders and modular arithmetic — More Operations
Standard long division yields a quotient and a remainder. The integer division operator // computes the quotient. The operator % computes the remainder.
For any integers a and b, a == b * (a // b) + (a % b).
In Python, a % b always returns an answer that is between 0 and b (even if a and/or b is negative).
Remainders and modular arithmetic are very useful in games for the purpose of "wrapping" the canvas, i.e; causing objects that pass off of one side of the canvas to reappear on the opposite side of the canvas.
Lecture examples - More operations
More examples - Modulus, Math Module,
Modules — More Operations
Modules are libraries of Python code that implement useful operations not included in basic Python.
Modules can be accessed via the import statement.
CodeSkulptor implements parts of the standard Python modules math and random.
Lecture examples - More operations
More examples - Math Module, Numbers and Strings, Random Module, Module Errors
Boolean Expressions — Logic and Comparisons
The constants True and False of the type bool.
These constants can be combined to form Boolean expressions via the logical operators and, or, and not.
The and of two Boolean expressions is True if both of the expressions are True.
The or of two Boolean expressions is True if at least one of the expressions is True.
Lecture examples - None
More examples - Booleans, Boolean Logic
Relational Operators — Logic and Comparisons
The values of two arithmetic expressions can be compared using the operators ==, !=, <, >, <=, >=.
These comparisons return either True or False .
Lecture examples - None
More examples - Comparison, Boolean Expressions
Conditional Statements — Conditionals
Conditional statements are compound statements consisting one or more clauses headed by the keywords if, elif, and else.
Each if or elif clause is followed by a Boolean expression and a colon :.
If the Boolean expression for a clause is True, the body of the clause is executed.
Lecture examples - Conditionals
More examples - if-elif-else, Examples of Conditionals
Programming Tips — Week 1


Week two Help Center

Event handlers — Event-driven programming
Event handlers (also called callbacks) are functions registered to an event such as a button click, keyboard press or mouse click.
Event handlers react to the event by changing the state (collection of information) encoded in the program.
Lecture examples - Events
More examples - None
Local variables — Local vs. global variables
Assignment to a variable inside a Python function creates a local variable.
The scope of variable (portion of the program where the value of the variable can be accessed) is the body of function.
Lecture examples - Local vs Global
More examples - Example
Global variables — Local vs. global variables
Variables defined outside functions are global variables. Their values may be accessed inside functions without declaration.
To modify to a global variable inside a function, the variable must be declared inside the function using the keyword global.
Global variables are a convenient (but dangerous) way for event handlers to share information in event-driven programming.
Lecture examples - Local vs Global
More examples - Example
SimpleGUI module — SimpleGUI
Special module for CodeSkulptor that supports 2D interactive applications. The Docs button links to documentation for SimpleGUI.
SimpleGUI allows creations of frames and timers as well as loading sounds and images.
Frames include a control panel (with buttons and input fields), a status area (for monitoring keyboard and mouse events) and a canvas (with simple 2D drawing operations).
Lecture examples - SimpleGUI, Template
More examples - Layout, Frame, Errors
Buttons — Buttons
Buttons may be created (and their event handlers registered) via add_button.
Buttons are positioned linearly (top/down) in the control panel in their order of creation.
Lecture examples - Calculator, Buttons
More examples - Structure, Canvas Color, Prize Boxes, True-False Quiz
Input fields — Input fields
Input fields may be created (and their event handlers registered) via add_input.
Input fields are positioned linearly (top/down) in the control panel in their order of creation.
The event handlers for the input field take a single parameter that is the text string entered.
Lecture examples - Calculator, Input Fields
More examples - Structure, Functions, Factoring, Silly Words
Programming Tips — Week 2


Week three Help Center

Canvas — Canvas and drawing
The canvas is the area associated with an application where information contain in the application may be drawn.
In SimpleGUI applications, the width and height of the canvas are specified (in pixels) in create_frame. (A pixel is the smallest unit of area that your computer can draw in.)
The origin for the canvas is the upper left-hand corner.
Positions in the canvas are specified as pairs [x,y] where x is the horizontal coordinate and y is the vertical coordinate.
Lecture examples - Canvas and Drawing
More examples - Structure
Event-driven drawing — Canvas and drawing
Computers refresh their screens around 60 times per sec.
For each application, the computer calls a special event handler, the draw handler, that is registered to the application.
In SimpleGUI, the draw handler is registered via set_draw_handler.
The draw handler can modify the canvas via simple draw operations defined in SimplGUI
Lecture examples - Canvas and Drawing
More examples - Structure, Echo
String operations — String processing
The function str converts other types of data into a string.
The concatenation operator + joins two strings to form a single string,
The ith element of a string my_string can be access via my_string[i]. Note that strings are immutable (cannot be changed).
Substrings of my_string can be accessed via slicing .
Lecture examples - Strings, Dollars and Cents One, Dollars and Cents Two
More examples - Operations, Input Checking, Initials
Drawing text — Interactive drawing
The method draw_text draws a string when given a position (lower left corner), a font size and a color.
The method draw_circle (see "More examples" below) draws a circle at a given point with a given radius in pixels. To draw a point, draw a circle of radius one.
The method draw_line (see "More examples" below) draws a line between two points.
The method draw_polygon (see "More examples" below) draws a sequence of points (enclosed in square brackets and separated by commas) as a closed polygon.
Colors for drawing methods can be specified as HTML color strings; "White", "Red", "Green", ...
Lecture examples - Drawing, Interactive Drawing
More examples - Shapes, Pictures, Hidden Picture
Timers — Timers
Timers are another component of SimpleGUI that generate regularly timed events.
Users create a timer using create_timer with a specified interval and event handler.
The timer calls its associated event handler regularly at the given interval.
A timer t is started with t.start() and is stopped by t.stop().
Lecture examples - Timers
More examples - Blinking Text, Reaction Time
Programming Tips — Week 3 (pt. 1), Week 3 (pt. 2)


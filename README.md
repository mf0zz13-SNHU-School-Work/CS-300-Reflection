# CS-300-Reflection
## What was the problem you were solving in the projects for this course?

The main problem I was solving was designing and implementing data structures and functions to assist academic advisors in managing and querying course data. This required building a system that could efficiently load, store, search, and display course information—including prerequisites—using appropriate data structures. The challenge was to create a maintainable and performant program that could handle common advisor tasks through a simple menu interface.

## How did you approach the problem? Consider why data structures are important to understand.

I approached the problem by first analyzing the nature of the data and operations involved. Since the course data required fast lookup, sorted output, and potential scalability, I implemented the system using three different data structures: a vector, a binary search tree (BST), and a hash table. Each structure provided different trade-offs:

- Vector: Simple to use and good for basic iteration and sorting.
- Binary Search Tree: Provided sorted output and efficient in-order traversal.
- Hash Table: Allowed fast insertion and lookup for course details.

## How did you overcome any roadblocks you encountered while going through the activities or project?

Some of the primary challenges included:

- Parsing complex CSV data: I resolved this by writing a custom parser that split lines based on commas and validated the structure before creating course objects.
- Ensuring case-insensitive search: I added logic to standardize input formatting before performing comparisons.
- Managing prerequisites: I implemented logic to validate and store prerequisite relationships without introducing invalid or missing references.

- Regular testing, using debug outputs, and breaking down functions into smaller components helped isolate and solve these issues.

## How has your work on this project expanded your approach to designing software and developing programs?

This project reinforced the importance of planning before coding. Writing pseudocode and selecting the right data structure up front made the implementation phase smoother. I was able to practice and reinforce my ability to:

- Break problems down into manageable functions
- Design systems that are modular and reusable
- Think through user experience even in CLI-based programs

It also emphasized the importance of error handling, especially when dealing with user input and file operations.

## How has your work on this project evolved the way you write programs that are maintainable, readable, and adaptable?

This project solidified several good programming habits:

- Consistent formatting and naming conventions for better readability
- Detailed comments and documentation to clarify function purposes and logic
- Modular design: Functions like `ParseFile`, `Add`, `Search`, and `PrintList` were kept focused and easy to test independently
- Scalability mindset: I structured the code so that switching data structures (e.g., swapping out the BST for a hash table) required minimal changes

Overall, I now place greater emphasis on writing code that others (or my future self) can understand, extend, and debug.

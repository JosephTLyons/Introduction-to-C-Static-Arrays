## Introduction to Static C++ Arrays
### What is an array?

What is an array and how is it useful?  By now, you have already discovered and used the various data types available in C++: int, char, float, and double.  In the most simple definition, arrays are just single structures that are capable of holding many instances of these data types.  For instance, a single character will not suffice if the user wishes to hold a static string of text, such as "Hello, World!"  Alternatively, it would be overkill to declare an individual variable for each character in the string.  Situations like these call for the use of an array.

### Declaration:
Declaring an array is fairly straight-forward:

1. Specify the data type (int, char, float, double)
2. Name the array
3. Give the array its size by placing the the size value inside of the subscript operator **[x]** (where x denotes the size of the array)
4. End with a statement terminator **;**

#### Examples of Declaring an Array:

- int myIntArray[5]; // Creates an array of 5 elements, ranging from indices 0 through 4 (More on this soon)
- char myCharArray[10]; // Creates an array of 10 elements, ranging from indices 0 through 9

Arrays can also be initialized the moment they are created as well via the initializer list.  Simple add an **=**, a pair of brackets **{}** and the list of numbers you would like to initialize the array to.  **NOTE** - it is important to know that the initializer list cannot be larger than the capacity of the array.


#### Examples of Initializing an Array Upon Declaration:

- int myIntArray[5] = {}; // Creates an empty array, where each element is a null terminator (More on this soon)
- char myCharArray[10] = {10, 9, 8, 7, 6, 5, 4, 3, 2, 1); // Creates an array with elements initialized to these values

### Accessing Contents of an Array:

Retrieving the contents of a single cell in an array, or the entire contents of the array, are both fairly easy tasks.  Before we can do that, we must know how the cells of the array are numbered.  Though one would probably be led to believe that the first element of an array is stored in cell one, this is actually not the case. The first element of an array is actually stored at cell 0.  This means that for any n element in the array, where n is the actual position, we would specify n - 1.  This means, if we want to access the first element of our array, we would actually specify cell 0.

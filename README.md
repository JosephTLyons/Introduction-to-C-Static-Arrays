## Introduction to Static C++ Arrays
### What is an array?

What is an array and how is it useful?  By now, you have already discovered and used the various data types available in C++: int, char, float, and double.  In the most simple definition, arrays are just single structures that are capable of holding many instances of these data types.  For instance, a single character will not suffice if the user wishes to hold a static string of text, such as "Hello, World!"  Alternatitely, it would be overkill to declare an individual variable for each character in the string.  Situations like these call for the use of an array.


### Declaration:
Declaring an array is fairly straight-forward:

1) Specify the data type (int, char, float, double)

2) Name the array

3) Give the array its size by placing the the size value inside of the subscript operator **[x]** (where x denotes the size of the array)

4) End with a statement terminator **;**

Examples:

int myInt[5];

char myChar[10];

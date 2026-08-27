# ECE-2112-PA-1
**Made by: Sophia Marielle R. Quizon | 2ECE-B**

The content of this repository contains the Programming Assignment for the course Advanced Computer Programming and Algorithms for the S.Y. 2026-2027.

# 1. Word Rotation Problem

The word rotation problem creates a function that accepts a string as input and moves its first character to the end of the string. This demonstrates how string slicing and indexing can be used in Python to manipulate text.

The function used for this problem is `rotate_word()`. It accepts one argument, which is the string that will be rotated. The function removes the first character from its original position and places it at the end of the string.


The following methods are used:

• `rotate_word()` - A user-defined function created to rotate the characters of a string.

• `text[1:]` - This is a string slicing method. It gets all the characters starting from index 1 until the end of the string. Since python starts counting at index 0, index 1 represents the second character.

• `text[0]` - A string indexing method that gets the first character of the string, which is located at index 0.

The operations were put together to produce the following function:

```def rotate_word (text): 
    return text [1:] + text [0]

print (rotate_word ("python"))
print (rotate_word ("logic"))
print (rotate_word ("code"))
print (rotate_word ("A"))




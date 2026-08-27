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

```python
def rotate_word (text): 
    return text [1:] + text [0]

Thank you for reading!

To fully see the main python program, please visit the link provided below:
https://github.com/alijahlazaga/ECE-2112-PA-1/blob/2504a5e6b50a3accfef0baf13a26f1c2e5f7766b/Programmingasiggnment1.ipynb

### **README file Version History:**

August 26, 2026 - initial README content uploaded

August 26, 2026 - Final README content added

print (rotate_word ("python"))
print (rotate_word ("logic"))
print (rotate_word ("code"))
print (rotate_word ("A"))
```

# 1. Username Builder Problem\

The username builder problem generates a username from a given first name and last name. The names are converted to lowercase, spaces are removed, and a period is placed between two names.

The operations were put together to produce the following function:

• `make_username(first_name, last_name)` - A user-defined function that receives two strings and formats them into one username.

• `.lower` - A string method that changes the uppercase characters into lowercase.

• `.replace(" ",")` - A string method that gets rid of spaces by replacing them with an empty string.

The complete function for the problem is:

```python
def make_username (first_name, last_name):

    first_name = first_name.lower()
    first_name = first_name.replace(" ","")

    last_name = last_name.lower()
    last_name = last_name.replace(" ","")

    return first_name + "." + last_name


print (make_username ("Ada", "Lovelace"))
print (make_username ("Alan", "Turing"))
print (make_username ("Ana Maris", "De Leon"))
```

# 3. Bookend Swap Problem

The bookend swap problem creates a function that switches the positions of the first and last elements of a list while leaving the elements in between unchanged.

The following functions were put together to produce the problem:

• `swap_bookends(items)` - A user-defined function that accepts a list, separates its elements into three parts, and exchanges the positions of the first and last elements.

• `first, *middle, last = items` - An extended unpacking operation that divides the list into three variables. The first item is stored in first, all elements between the two ends are placed in middle, and the final item is stored in last.

• `return [last] + middle + [first]` - Creates the resulting list by putting the original last element at the beginning and the original first element at the end, while retaining the middle elements in the same arrangement.

The combination of the different operations gives the final function:

```python
def swap_bookends(items): 
    first, *middle, last = items
    return [last] + middle + [first]

print (swap_bookends ([1, 2, 3, 4, 5, 6]))
print (swap_bookends (["red", "green", "blue"]))
print (swap_bookends ([8, 3]))
```

Thank you for reading!

For reference of the main python program for Programming Assignment 1, kindly click the link and download:
https://github.com/sphmrlle/ECE-2112-PA-1/blob/main/PA1_Quizon.ipynb 

### **README file Version History:**

August 25, 2026 - Initial README ouput uploaded

August 26, 2026 - Draft for README was plotted

August 27, 2026 - Final README updated



# ECE2112_PA1

Adrian Jomer V. Arboso
2ECE-D

### ALPHABET SOUP PROBLEM:
 1. Create a function that takes a string and returns a string with its letters in alphabetical order.
Example: alphabet_soup(“hello”) ➞ ehllo
alphabet_soup(“hacker”) ➞ acehkr

Code:
![image](https://github.com/user-attachments/assets/5655905b-226b-43eb-8286-b2c9c78f165b)

 

Output:
ehllo
acehkr

### EMOTICON PROBLEM: 
Create a function that changes specific words into emoticons. Given a sentence 
as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:

Example:
emotify(“Make me smile”) ➞ Make me :)
emotify(“I am mad”) ➞ I am >:(

Code:
![image](https://github.com/user-attachments/assets/93d22fbb-7701-4c5f-8471-8d080928f15b)



Sample output:

Enter a Sentence: Make me sad
output:

Make me :((

### UNPACKING LIST PROBLEM: 
Unpack the list writeyourcodehere into three variables, being first,
middle, and last, with middle being everything in between the first and last element. Then print all three 
variables.

Example: lst = [1, 2, 3, 4, 5, 6]
Output: first: 1 middle: [2,3,4,5] last: 6

Code:
![image](https://github.com/user-attachments/assets/46518131-2069-4e47-bd3f-50707c4131cd)

Output: 
first: 1
middle: [2,3,4,5,6]
last: 7

Simce I was not able to put comments in the problem 3, I will just explain it here:

For line 1-7: First, initialize a list of numbers, then set the starting index to 1. Next, initialize an empty list to store selected elements, and finally, append the string "end" to the end of the list.

For line 8-15: A while loop that copies elements lst to lsts starting from index 1 until it encounters "end". When "end" is found, the loop removes the last added element, adjusts the index, and then breaks the loop.

For line 17-19: Display the 1st, middle and last.

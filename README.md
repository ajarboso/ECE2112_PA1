# ECE2112_PA1

Adrian Jomer V. Arboso
2ECE-D

ALPHABET SOUP PROBLEM:
 1. Create a function that takes a string and returns a string with its letters in alphabetical order.
Example: alphabet_soup(“hello”) ➞ ehllo
alphabet_soup(“hacker”) ➞ acehkr

Code:
def alphabet_soup(s):
    sorted_s = ""  # Initialize an empty string to store the sorted characters

    # Continue until the string is empty
    while s: 
        # Find the smallest character in the string
        x = min(s) 
         # Add all occurrences of that character to the sorted string
        sorted_s += x * s.count(x)  
        # Remove all occurrences of the character from the string
        s = s.replace(x, '')
    
    return sorted_s  # Return the sorted string

print(alphabet_soup("hello"))
print(alphabet_soup("hacker"))

Output:
ehllo
acehkr

EMOTICON PROBLEM: 
Create a function that changes specific words into emoticons. Given a sentence 
as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:

Example:
emotify(“Make me smile”) ➞ Make me :)
emotify(“I am mad”) ➞ I am >:(

Code:

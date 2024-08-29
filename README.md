# ECE2112_PA1

Adrian Jomer V. Arboso
2ECE-D

ALPHABET SOUP PROBLEM:
 1. Create a function that takes a string and returns a string with its letters in alphabetical order.
Example: alphabet_soup(“hello”) ➞ ehllo
alphabet_soup(“hacker”) ➞ acehkr

Code:

 
 #Initialize an empty string to store the sorted characters
 def alphabet_soup(s):
    sorted_s = "" 
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
ef replace_emoticons(sentence):
    # Dictionary mapping words to their corresponding emoticons
    d = {
        "smile": ":)", 
        "grin": ":D",
        "sad": ":((",
        "mad": ">:("
    }
    
    # Check if any keyword exists in the sentence and replace it with its corresponding emoticon
    if "smile" in sentence:
        sentence = sentence.replace("smile", d["smile"])
    elif "grin" in sentence:
        sentence = sentence.replace("grin", d["grin"])
    elif "sad" in sentence:
        sentence = sentence.replace("sad", d["sad"])
    elif "mad" in sentence:
        sentence = sentence.replace("mad", d["mad"])
        
    # Return the modified sentence 
    return sentence    
user_input = input("Enter a sentence: ")
result = replace_emoticons(user_input)
print(result) 


Sample output:

Enter a Sentence: Make me sad
output:

Make me sad :((

UNPACKING LIST PROBLEM: 
Unpack the list writeyourcodehere into three variables, being first,
middle, and last, with middle being everything in between the first and last element. Then print all three 
variables.

Example: lst = [1, 2, 3, 4, 5, 6]
Output: first: 1 middle: [2,3,4,5] last: 6

Code:

# Regex in Python: Filter Words Without the Letter 'e'
## NAME: JANARTHANI R
## REF NO: 25017541
## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
import re

items=['goal','new','user','sit','eat','dinner']

filtered_list=[]

for word in items:

  if not re.search('e',word):

     filtered_list.append(word)

print("Original list:",items)

print("Filtered list (without 'e'):",filtered_list)
## Output
Original list: ['goal','new','user','sit','eat','dinner']

Filtered list (without 'e'): ['goal','sit']
## Result
The program successfully filters and returns all words that do not contain the letter 'e' using regular expressions. Only the words that satisfy the condition are displayed in the final list.

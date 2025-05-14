# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim:
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm:
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program:
```
import re
words = ["apple", "banana", "cherry", "fig", "grape", "kiwi", "mango"]
def filter_without_e(word_list):
    # Match only words that do NOT contain 'e' (case-insensitive)
    pattern = re.compile(r'^[^eE]*$')
    return [word for word in word_list if pattern.match(word)]
filtered_words = filter_without_e(words)
print("Words without the letter 'e':", filtered_words)
```
## Output:
```
     Input                  Result
apple 
banana
cherry
fig                        Words without the letter 'e': ['banana', 'fig', 'kiwi', 'mango']
grape
kiwi
mango
```
## Result:
The program  was successful.

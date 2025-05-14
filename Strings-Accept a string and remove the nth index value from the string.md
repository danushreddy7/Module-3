# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python program that accepts a string and removes the character at a specified index.

## 🧠 Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## 💻 Program
```
def remove_char_at_index(s, index):
    if index < 0 or index >= len(s):
        return "Index out of range"
    return s[:index] + s[index+1:]
input_str = input("Enter a string: ")
index = int(input("Enter the index of the character to remove: "))
result = remove_char_at_index(input_str, index)
print("Resulting string:", result)
```
## Output:
```
Enter a string: hello
Enter the index of the character to remove: 1
Resulting string: hllo
```
## Result:
The program was successful.

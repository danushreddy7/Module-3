# Tuple in Python: Check Element Existence

## 🎯 Aim
To write a Python program that checks if the element `'n'` and the element `8` exist within a given tuple.

## 🧠 Algorithm
1. Define a tuple `x` with some letters and numbers.
2. Use the `in` operator to check if the string `'n'` exists within the tuple.
3. Use the `in` operator to check if the integer `8` exists within the tuple.
4. Print the results.

## 🧾 Program
```
my_tuple = ('a', 'b', 'n', 3, 8, 'z')
element1 = 'n'
element2 = 8
if element1 in my_tuple and element2 in my_tuple:
    print(f"Both '{element1}' and {element2} are present in the tuple.")
else:
    print(f"Either '{element1}', {element2}, or both are not present in the tuple.")
```
## Output: 
```
       Input                                              Result

('a', 'b', 'n', 3, 8, 'z')                  Both 'n' and 8 are present in the tuple
```
## Result:
The program was successful.

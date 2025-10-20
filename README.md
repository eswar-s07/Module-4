# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program

```
import math
radius=float(input())
class cse:
    def __init__(self,radius):
        self.r=radius
    def mech(self):
        area=math.pi*self.r*self.r
        return area
o=cse(radius)
print("Area of circle :",o.mech())
```

## Output
![alt text](<Screenshot 2025-10-20 105250.png>)

## Result
Thus the program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation is executed successfully.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program

```
dict1 = {
    'name': 'Alice',
    'age': 30,
    'city': 'New York',
    'job': 'Engineer'}
dict2 = {
    'age': 32,
    'job': 'Data Scientist',
    'salary': 75000
}
def merge():
    merged_dict={**dict1,**dict2}
    return merged_dict
print("merged dictionary :",merge())
```

## Output
![alt text](<Screenshot 2025-10-20 110308.png>)

## Result
Thus the program that merges **two dictionaries** and combines their key-value pairs is executed successfully.

# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program

```
dict1 = {
    'banana': 3,
    'apple': 1,
    'orange': 4,
    'grape': 2,
    'kiwi': 5
}
sortedkey_list=sorted(dict1.items())
sortedkey_dict=dict(sortedkey_list)
sortedval_list=sorted(dict1.items(),key=lambda item:item[1])
sortedval_dict=dict(sortedval_list)
print("Original dict :",dict1)
print("Sorted by keys :",sortedkey_dict)
print("Sorted by values :",sortedval_dict)
```

## Sample Output
![alt text](<Screenshot 2025-10-20 111211.png>)

## Result
Thus the program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order
is executed successfully.

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program

```
list1=[15,64,8,1,56]
try:
    print(list1[2])
    print(list1[5])
except:
    print("You're out of list range")
```

## Output
![alt text](<Screenshot 2025-10-20 111436.png>)

## Result
Thus the program that handles an **IndexError** when trying to access an element beyond the available range of a list is executed successfully.

# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program

```
import re
with open('story.txt','r') as r:
    count=0
    lines=r.readlines()
    for i in lines:
        if re.match('[Tt]',i):
            pass
        else:
            count+=1
    print(count)
```

## Output
![alt text](<Screenshot 2025-10-20 112549.png>)

## Result
Thus the program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'` is executed successfully.
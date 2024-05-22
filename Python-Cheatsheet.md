# Python Coding Interview Cheatsheet

## Lists (Arrays)
### Initialization
- **Definition**: Lists are ordered, mutable collections of items.
- **Usage**: `nums = [1, 2, 3]`
  - Creates a list with elements 1, 2, and 3.
  - Lists can hold items of different data types, though typically they hold similar types for consistency.

### Dynamic Arrays
- **Definition**: Lists in Python are dynamic, meaning they can grow and shrink in size.
- **Usage**:
  ```python
  nums.append(4)  # Adds element 4 to the end of the list
  nums.pop()  # Removes and returns the last element (4 in this case)
  ```
  - `append` is used to add an item to the end of the list.
  - `pop` is used to remove the last item from the list.

### Slicing
- **Definition**: Accessing a subset of the list using indices.
- **Usage**: `nums[1:3]` (returns elements at index 1 and 2)
  ```python
  nums = [1, 2, 3, 4]
  sliced = nums[1:3]  # Result: [2, 3]
  ```
  - Slicing allows you to create a new list from an existing one, starting at the first index and up to but not including the second index.

### List Comprehension
- **Definition**: A concise way to create lists.
- **Usage**: `[i for i in range(5)]` (creates `[0, 1, 2, 3, 4]`)
  ```python
  squares = [i*i for i in range(5)]  # Result: [0, 1, 4, 9, 16]
  ```
  - List comprehensions provide a concise way to create lists from sequences.

### Unpacking
- **Definition**: Assigning elements of a list to multiple variables.
- **Usage**: `a, b, c = [1, 2, 3]`
  ```python
  nums = [1, 2, 3]
  a, b, c = nums  # a=1, b=2, c=3
  ```
  - Useful for quickly assigning values without needing to access indices individually.

## Strings
### Initialization
- **Definition**: Strings are immutable sequences of characters.
- **Usage**: `s = "hello"`
  - Creates a string with the text "hello".

### Slicing
- **Definition**: Accessing a subset of the string.
- **Usage**: `s[1:3]` (returns characters at index 1 and 2)
  ```python
  s = "hello"
  sliced = s[1:3]  # Result: "el"
  ```

### Immutable
- **Definition**: Strings cannot be changed after they are created.
- **Usage**:
  ```python
  s = "hello"
  s = s + " world"  # Creates a new string "hello world"
  ```
  - To change a string, you must create a new one.

### Conversion
- **Definition**: Changing data types to/from strings.
- **Usage**:
  ```python
  num = int("123")  # Converts string "123" to integer 123
  s = str(123)  # Converts integer 123 to string "123"
  ```

## Tuples
### Initialization
- **Definition**: Tuples are immutable, ordered collections of items.
- **Usage**: `t = (1, 2, 3)`
  - Creates a tuple with elements 1, 2, and 3.

### Immutability
- **Definition**: Tuples cannot be changed after creation.
- **Usage**:
  ```python
  t = (1, 2, 3)
  # t[0] = 0  # This will raise an error because tuples are immutable
  ```

### Use in Dictionaries
- **Definition**: Tuples can be used as keys in dictionaries.
- **Usage**:
  ```python
  d = {(1, 2): "a pair"}  # Tuples as keys
  ```

## Dictionaries (HashMaps)
### Initialization
- **Definition**: Dictionaries are mutable collections of key-value pairs.
- **Usage**: `d = {"a": 1, "b": 2}`
  - Creates a dictionary with keys "a" and "b" mapped to values 1 and 2, respectively.

### Access
- **Definition**: Retrieve a value by its key.
- **Usage**: `d["a"]` (returns `1`)
  ```python
  value = d["a"]  # Result: 1
  ```

### Modify
- **Definition**: Change the value associated with a key.
- **Usage**: `d["a"] = 10`
  ```python
  d["a"] = 10  # Changes the value of key "a" to 10
  ```

### Remove
- **Definition**: Delete a key-value pair.
- **Usage**: `del d["a"]`
  ```python
  del d["a"]  # Removes the key "a" and its value from the dictionary
  ```

### Comprehension
- **Definition**: A concise way to create dictionaries.
- **Usage**: `{i: i*2 for i in range(3)}` (creates `{0: 0, 1: 2, 2: 4}`)
  ```python
  doubled = {i: i*2 for i in range(3)}  # Result: {0: 0, 1: 2, 2: 4}
  ```

## Sets
### Initialization
- **Definition**: Sets are unordered collections of unique items.
- **Usage**: `s = {1, 2, 3}`
  - Creates a set with elements 1, 2, and 3.

### Add/Remove
- **Definition**: Add or remove items from a set.
- **Usage**:
  ```python
  s.add(4)  # Adds 4 to the set
  s.remove(3)  # Removes 3 from the set
  ```

### Comprehension
- **Definition**: A concise way to create sets.
- **Usage**: `{i for i in range(5)}`
  ```python
  squares = {i*i for i in range(5)}  # Result: {0, 1, 4, 9, 16}
  ```

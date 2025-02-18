# Python lecture 4

## List Comprehensions

```python
lst = [x for x in 'word']
```

output:
['w','o','r','d']

```python
lst = [x**2 for x in range(0,11)]

```

```Python
lst = [x for x in range(11) if x % 2 == 0]
prints evens from 0 to 10

```

```Python
celcius = [0,10,20.1, 34.5]

farenheit = [ ((float(9)/5)* temp + 32) for temp in celsius]

output:
[32.0, 50.0, 68.18, 94.1]

```

```Python

lst = [x**2 for x in [x**2 for x in range(11)]]
lst

output:
[0,1,16,81,256,1296,2401,4096,6561,10000]

```

- [] Change power of x to see changes

## Dictionary

- Can have different data types
- Has its own methods

```Python
my_dict = {'key1': 'value1', 'key2': 'value2'}


```

- Can think about it as an array
- Can nest dictionaries
- items() returns tuples
- Turn dictionary into a set and avoid redundancy

| Method         | Description                                                                                                 |
| -------------- | ----------------------------------------------------------------------------------------------------------- |
| `clear()`      | Removes all the elements from the dictionary                                                                |
| `copy()`       | Returns a copy of the dictionary                                                                            |
| `fromkeys()`   | Returns a dictionary with the specified keys and value                                                      |
| `get()`        | Returns the value of the specified key                                                                      |
| `items()`      | Returns a list containing a tuple for each key-value pair                                                   |
| `keys()`       | Returns a list containing the dictionary's keys                                                             |
| `pop()`        | Removes the element with the specified key                                                                  |
| `popitem()`    | Removes the last inserted key-value pair                                                                    |
| `setdefault()` | Returns the value of the specified key. If the key does not exist: insert the key, with the specified value |
| `update()`     | Updates the dictionary with the specified key-value pairs                                                   |
| `values()`     | Returns a list of all the values in the dictionary                                                          |

- [ ] Update Faculty_language function in the notebook from lecture

```Python
# Correct way to grow dictionaries

dict5 = {}

dict5['k1'] = 'Hello'

dict['k3'] = 'world'

```

## Tuples

```Python
# Create Tuples

t = (1, 2, 3)

# Check length

len(t)

# Mix type

t = ('one', 2)

```

| Method | Description                              |
| ------ | ---------------------------------------- |
| index  | Enter a value and return the index       |
| count  | Count the number of times shown in tuple |

> [!IMPORTANT]
> Quiz One week from today
> Tue 18
> Lists
> Tuples

> [!IMPORTANT]
> Quiz two
> Wed 20

> Dictionaries

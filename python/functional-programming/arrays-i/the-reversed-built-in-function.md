---
author: stefkn
type: normal
category: must-know
links:
  - >-
    [Python
    reversed()](https://www.programiz.com/python-programming/methods/built-in/reversed){website}
practiceQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
---

# The reversed Function


---

## Content

The `reversed` function takes in an iterable object, like a string or a list, and returns an iterator for the sequence in the reversed order.

```python
ourString = 'enki'
print(list(reversed(ourString)))
# Result: ['i', 'k', 'n', 'e']

ourList = [1,2,3,4]
print(list(reversed(ourList)))
# Result: [4, 3, 2, 1]

ourTuple = ("Hello", "World")
print(list(reversed(ourTuple)))
# Result: ["World", "Hello"]
```

We can even use `reversed` on custom objects! [1]

---

## Practice

Fill in the blanks to reverse the order of the list `ourList`.

```python
ourList = [5, 4, 3, 2, 1]
newList = ???(???(???))
```

- `list`
- `reversed`
- `ourList`
- `newList`
- `seq`
- `__reversed__`


---

## Revision

Fill in the blanks so that the following custom class properly implements `__reversed__()`, so that `reversed` can be used on instances of the class.

```python
class Classroom:
    pupils = ['bob', 'joe', 'anne']

    def __reversed__(self):
        return ???(???.???)

c = Classroom()
print(list(reversed(c)))
```

- `reversed`
- `self`
- `pupils`
- `Classroom`
- `bob`
- `__len__()`


---

## Footnotes

[1:`__len__ and __getitem__`]
For `reversed` to work, the object passed in must either:
- implement the `__reversed__()` method
- implement both the `__len__()` and `__getitem__()` methods with integer arguments.


Notice how we could create custom classes that implement the `__reversed__()` method and then use `reversed` on them to quickly and efficiently reverse their ordering. 
 
---
author: lior-bd
type: normal
category: must-know
links:
  - >-
    [Python
    slice()](https://www.programiz.com/python-programming/methods/built-in/slice){website}
practiceQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
---

# Advanced slice

---

## Content


We can also use **negative numbers** as arguments to `slice`, which will count indexes in reverse order.

```python
ourList = ["A", "B", "C", "D", "E"]
sObject = slice(-1, -4, -1)
print(ourList[sObject])
# Result: ["E", "D", "C"]
```

The above code: 
- Starts at `-1`, which will be the last element, `"E"`.
- Stops before `-4`, which will be the fourth to last element, `"B"`.
- Increments at `-1`, which means it iterates `1` to the left[1] each time.

---

## Practice

Use `slice` to extract the substring 'spam' from 'spam-eggs-ham-chips' by filling in the gaps.

```python
ourString = 'spam-eggs-ham-chips'

sObject = ???(???)
print(ourString[sObject])
```

- `slice`
- 4
- 5
- 3
- `list`


---

## Revision

Use `slice` to remove every second number in the list of numbers.

```python
nList = ['1', '2', '3', '4', '5', '6', '7', '8']

sObject = ???(???, ???, ???)
print(nList[sObject])
```

- slice
- 1
- 8
- 2
- 3
- 7
- seq


---

## Quiz

### how does slicing work?


What will be printed by the following snippet?

```python
a = 'enki'
print(a[::-1])
```

 ???

- ikne
- i
- enki
- TypeError: str object is not subscriptable


---

## Footnotes

[1:Negative Increments]
Negative steps iterate backwards through the list, instead of forwards.

Since a step of `2` iterates every other element to the right, a step of `-2` iterates every other element to the left.

 
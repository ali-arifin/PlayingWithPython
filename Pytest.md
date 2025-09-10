# Pytest

[Unittests](https://github.com/ali-arifin/PlayingWithPython/blob/main/UnitTest.md) use an object-oriented approach to write tests, while pytests use a functional approach. Pytests use built-in assert statements, making tests easier to read and write.

Below is a file called ```math_operations.py```
```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b
```

Below is a file called ```test_math_operations.py```

```python
from math_operations import add, subtract

def test_add():
    assert add(2, 3) == 5
    assert add(-1, 1) == 0

def test_subtract():
    assert subtract(5, 3) == 2
    assert subtract(0, 4) == -4

def test_add_fail():
    assert add(2, 2) == 5  # 2 + 2 is 4, so this should fail
```

To run the test, we go the terminal and run this command:

<img width="1392" height="607" alt="image" src="https://github.com/user-attachments/assets/d81db508-0b23-4386-917c-11edc35908ee" />

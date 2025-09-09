# Unit Test
A test to verify that small isolated parts of a program work correctly

The ```unittest``` module in Python is a built-in testing framework that allows you to write and run tests for your code.

```python
import unittest

# Function to be tested
def add(a, b):
    return a + b

# Test Case Class
class TestAddFunction(unittest.TestCase):

    def test_add_positive_numbers(self):
        self.assertEqual(add(2, 3), 5) # ✅ Passes

    def test_add_negative_numbers(self):
        self.assertEqual(add(-1, -1), -2) # ✅ Passes

    def test_add_zero(self):
        self.assertEqual(add(0, 5), 5) # ✅ Passes

# Run the tests now — but only if this script is run directly, not if someone else imports this file
if __name__ == "__main__":
    unittest.main()

```

<img width="615" height="222" alt="image" src="https://github.com/user-attachments/assets/8879aee3-e01e-4500-a36c-87e08408a356" />


```python
import unittest

# Function to be tested
def add(a, b):
    return a + b

# Test cases
class TestAddFunction(unittest.TestCase):

    def test_add_positive_numbers(self):
        self.assertEqual(add(2, 3), 5)  # ✅ Passes

    def test_add_negative_numbers(self):
        self.assertEqual(add(-1, -1), -2)  # ✅ Passes

    def test_add_zero(self):
        self.assertEqual(add(0, 5), 5)  # ✅ Passes

    def test_wrong_answer(self):
        self.assertEqual(add(10, 5), 20)  # ❌ Fails

# Run the tests now — but only if this script is run directly, not if someone else imports this file
if __name__ == "__main__":
    unittest.main()
```

<img width="881" height="415" alt="image" src="https://github.com/user-attachments/assets/05fcce1e-7f80-4f17-8865-5d1c0b74a1a6" />


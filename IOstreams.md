# I/O Streams

I/O streams refer to data channels used for Input and Output operations. These channels allow your program to read from or write to various sources — like files, screen, keyboard, network sockets, etc.

## Python's Built-in Streams (via sys module):

<img width="932" height="215" alt="image" src="https://github.com/user-attachments/assets/75eb053d-b762-4f88-b0b8-68433a6c9858" /> 

<hr style="border-top: 3px double #bbb; margin: 20px 0;" />


```python
import sys

print("Type something and press Enter:")
user_input = sys.stdin.readline()  # reads one line from input stream
print("You typed:", user_input)
```

<img width="586" height="140" alt="image" src="https://github.com/user-attachments/assets/9052f60f-941e-4e7e-8e5b-afe3f2a2fcbf" />

<hr style="border-top: 3px double #bbb; margin: 20px 0;" />

```python
import sys

sys.stdout.write("This goes to standard output (stdout)\n")
sys.stderr.write("This goes to standard error (stderr)\n")
```

<img width="853" height="170" alt="image" src="https://github.com/user-attachments/assets/9dd6d18f-6d54-4160-83cc-05cdaf58aebc" />

<img width="424" height="106" alt="image" src="https://github.com/user-attachments/assets/1c99e3de-8302-43b9-9fd7-9dfde0f2fbfd" />

<img width="413" height="104" alt="image" src="https://github.com/user-attachments/assets/b3be7438-37d3-443f-9486-811444c2d629" />




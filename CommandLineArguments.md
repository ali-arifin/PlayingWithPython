# Command Line Arguments - using the ```sys``` module

```python
import sys
print(sys.argv)
```

This prints the list of command-line arguments passed to the Python script.

```sys.argv``` is a list from the sys module that contains:

- The name of the script (always ```argv[0]```)

- Followed by any arguments passed to the script on the command line

<img width="657" height="142" alt="image" src="https://github.com/user-attachments/assets/57c881be-b02c-4855-9222-c4c3c01503b4" />

<hr style="border-top: 3px double #bbb; margin: 20px 0;" />

The script below checks whether a file exists, otherwise it creates that file:

```python
import os
import sys

filename = sys.argv[1]

if not os.path.exists(filename):
    with open(filename, "w") as f:
        f.write("New file created\n")
else:
    print("Error, the file {} already exists!".format(filename))
    sys.exit(1)
```


<img width="725" height="124" alt="image" src="https://github.com/user-attachments/assets/c935e2ee-2b30-4aeb-9288-4f831c21fe6b" />

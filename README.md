# command-line-arguments-to-count-word

## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.

## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7

## ALGORITHM: 

### Step 1:
Import sys module to use command line arguments.

### Step 2: 
Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument.
 
### Step 3: 
Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument.

### Step 4:  
Split the contents into each line using .split() function.

### Step 5: 
Iterate the list of lines and increment the value of variable (word) each time.

### Step 6: 
Run the program by giving "python prgm.py EX12.txt" on the terminal.


## PROGRAM:
```
Developed By: Sivaramakrishnan B
Register Number: 212222110044

import sys
count = {}
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
print(count)
f.close()

```

### FILE CONTENT:
![image](https://github.com/SivaramakrishnanBaskar/command-line-arguments-to-count-word/assets/119476322/00cd34c6-dc7b-4225-a2aa-e6e25a13629f)

### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/command-line-arguments-to-count-word/assets/119476322/305fdeaa-113e-4418-921a-3e5bb0ed5a5d)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.

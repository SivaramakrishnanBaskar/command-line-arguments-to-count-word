# command-line-arguments-to-count-word

## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.

## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7

## ALGORITHM: 

### Step 1:
Get the file name using command arguments

### Step 2: 
Now read the content in the file
 
### Step 3: 
use split()

### Step 4:  
Now read the no.of words in file

### Step 5: 
Print number of words present in given file

### Step 6: 
End of the program

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

### OUTPUT:
![214607930-ccb4dd15-6e05-43e9-807d-3d97808296b2](https://github.com/SivaramakrishnanBaskar/command-line-arguments-to-count-word/assets/119476322/c0a1fd6a-2c15-4711-85d8-877d4d69b813)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.

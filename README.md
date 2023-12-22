# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 

### Step 1:
Import the sys module.

### Step 2: 
Pass the filename as the first argument after the name of script. Open the file as sys.argv[1]

### Step 3:
Read the file using read() method.

### Step 4: 
Use split() method to split the file content into words.

### Step 5: 
Use len() to find the total words.

### Step 6:
Use len() to find the total words.

## PROGRAM:
```
Program for getting the word count from the contents of a file using command line arguments
Developed by: BALAMURUGAN B
Register Number: 212222230016

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
![5b](https://github.com/BALA291/command-line-arguments-to-count-word/assets/120717501/04175a22-50c1-4f4b-b92b-07a189e8ffbe)
![5b file](https://github.com/BALA291/command-line-arguments-to-count-word/assets/120717501/6d7b4578-91c2-41a1-aee5-7e79604117db)
![5b out1](https://github.com/BALA291/command-line-arguments-to-count-word/assets/120717501/cc00e81e-b787-44e0-abc6-b800267c45bf)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.

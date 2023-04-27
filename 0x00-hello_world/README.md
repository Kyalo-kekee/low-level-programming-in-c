# QUESTIONS


## 0.Preprocessor

-Write a script that runs a C file through the preprocessor and save the result into another file.
-The C file name will be saved in the variable $CFILE
-The output should be saved in the file c.
==========================================================
### workflow
- create a file main.c `cat main.c`
write  c code in main.c
```C
#include <stdio.h>

/**
 * main - Entry point
 *
 * Return: Always 0 (Success)
 */
int main(void)
{
    return (0);
}


- use shell command `shell export CFILE= main.c 
- finally your 0.preprocessor file write the shell script that runs main.c thorugh the preprocessor

```bash
#!/bin/bash 

gcc -E CFILE -o c

=======================================================================================
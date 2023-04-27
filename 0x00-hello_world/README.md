# 0x00. C - Hello, World
## QUESTIONS


## 0-Preprocessor

Write a script that runs a C file through the preprocessor and save the result into another file.

The C file name will be saved in the variable $CFILE

The output should be saved in the file c.

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
```

- use bash command `export CFILE= main.c` 
- finally your 0.preprocessor file write the shell script that runs main.c thorugh the preprocessor

```bash
#!/bin/bash 
gcc -E CFILE -o c
```
## 1. Compiler 
Write a script that compiles a C file but does not link.

- The C file name will be saved in the variable $CFILE
- The output file should be named the same as the C file, but with the extension .o instead of .c

## workflow 

write a bash script that exports main.c to a variable CFILE. `export CFILE=main.c`

in the 1-compile file, write the script to compile script but not link

```
#!/bin/bash/
gcc -c CFIE 
```
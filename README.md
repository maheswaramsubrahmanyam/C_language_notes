C First Program

In the previous lesson, we learned how to set up the environment for C. Now, we will see how to run C first program.  It’s quite easy. Let’s begin with launching Turbo C and running C first program.

Go to Start > Turbo C

Open Turbo C and open a new project,

File > New


#include <stdio.h>
 
int main()
{
   printf("Studyopedia C Language Tutorial"); 
 
   return 0;
}
 
Here,

#include

It is the preprocessor and the first word read by the compiler

stdio.h

It is the header file.

int main()

main() function with return type int.

printf
Used to print the formatted string to stdout. The standard output is stdout.

return

Terminates the function execution and the return statement returns the control to the calling function.

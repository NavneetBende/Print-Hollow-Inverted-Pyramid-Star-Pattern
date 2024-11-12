PRINTING PATTERN:
*******

  *      *

    *  *

      *

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=r to i>0. The loop should be structured as for( i=r ; i>0 : i–).
 Run a nested loop inside the main loop to print the spaces before the pyramid. From k=r to k>i +1. The loop should be structured as for( k=r; k>i+1 ;k–).
Inside this nested loop print white space.
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=0 to j<i*2-1. The loop should be structured as for( j=0 ; j<i*2-1; j++).
Print star under the if condition (i==r).
Under the else condition  use another if condition to print the rest of the stars.
Use if(j==0 || j==i*2-2) to print stars.
Else print white space
In the main loop print a new line to move to the next line.
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,k,r;    //declaring integer variables i,j,k for loops and r for number of rows
printf("Enter the number of rows :\n");     //Asking user for input
scanf("%d",&r);      //saving number of rows in variable r
for(i=r;i>0;i--)    //outer loop for number of rows
   {
      for(k=r;k>i;k--)      //nested loop for spaces before the pyramid
         {
            printf(" ");     //printing white space
         }
      for(j=0;j<i*2-1;j++)      //loop for printing stars
         {
            if(i==r)      //condition to print the first row
               {
                  printf("*");     //printing stars in the first row
               }
            else     //else condition for printing the rest of the pyramid
               {
                  if(j==0||j==i*2-2)     //if condition to print the starting and ending stars in a row
                     {
                        printf("*");      //printing stars
                     }
                  else      //else condition for printing white space
                     {
                        printf(" ");     //printing white space
                     }
                }
          }
      printf("\n");     //printing newline after each row
   }
}
TAKING INPUT:

DISPLAYING OUTPUT:



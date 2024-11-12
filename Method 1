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

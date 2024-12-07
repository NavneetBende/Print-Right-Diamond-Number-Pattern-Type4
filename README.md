PRINTING PATTERN:
3

44

555

6666

555

44

3

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r. The loop should be structured as for( i=0 ; i
Use an if condition to to print the top half of the pyramid. if (i<=r/2). Then run a loop from j=0 to j<=i. The loop should be structured as for(j=0 ; j<=i ; j++)
Inside this loop print i+3.
Else run a different loop from j=i to jThe loop should be structured as for( j=i ; j
Inside this loop print (r-i+2).
Inside the main loop print a newline to move to the next line after each row is printed.
Input:
              3  4
Output:
               3
              44
              555
              6666
              555
              44
              3

Input :
              4  4
Output:
              4
              55
              666
              7777
              666
              55
              4

Code 1
#include<stdio.h>
int main()
{
  int i,j,s,N,count=0;
  scanf("%d%d",&s,&N);
    for(i=s;count<4;count++)
    {
      for(j=0;j<count+1;j++)
        printf("%d",i);
      printf("\n");
      i=i+1;
    }
    for(i=s+N-2;count>0;count--)
    {
      for(j=0;j<count-1;j++)
        printf("%d",i);
      printf("\n");
      i=i-1;
     }
  return 0;
}

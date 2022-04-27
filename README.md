# PPS_CLAP_1
#include <stdio.h>
int main()
{
  int i, n;
 
  int t1 = 0, t2 = 1; // initialize first and second terms

  int nextTerm = t1 + t2; // initialize the next term (3rd term)

  printf("Enter the number of terms: ");
  scanf("%d", &n); // get no. of terms from user

  printf("Fibonacci Series: %d, %d, ", t1, t2); // print the first two terms t1 and t2

  for (i = 3; i <= n; ++i) // print 3rd to nth terms
  {
    printf("%d, ", nextTerm);
    t1 = t2;
    t2 = nextTerm;
    nextTerm = t1 + t2;
  }

  return 0;
}

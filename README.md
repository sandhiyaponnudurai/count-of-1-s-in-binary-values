// count-of-1-s-in-binary-values
#include<stdio.h>

int main() {
   int n,x,a[10],count=0,i=0;
   scanf("%d",&n);
   while(n>0)
   {
       a[i++]=n%2;
       n=n/2;
       x=i;
   }
   for(i=x-1;i>=0;i--)
   {
       if(a[i]==1)
       {
           count++;
       }
   }
   printf("%d",count);
}

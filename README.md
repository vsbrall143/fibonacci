#include <stdio.h>
#include <stdlib.h>


int num,i,n;
void main()

{
    printf("enter number you want to get series for");
    scanf("%d", &num);

    for (i = 0; i < num; i++)
    {
        printf("%d", fab(i));
    }
}

void fab(n)
{
    if (n == 0)
        return 0;
    
    else if (n == 1)
        return 1;
    else
        return fab(n - 1) + fab(n - 2);
}

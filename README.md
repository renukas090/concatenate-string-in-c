# concatenate-string-in-c
/* write a program to concatenate string with or without strcat() function in C*/

#include <stdio.h>
#include<string.h>
#define N 200

int main()
{
    char a[N],b[N];
    int len1,len2,i;

    printf("Enter String");
    fgets(a,200,stdin);
    fgets(b,200,stdin);
    len1 = strlen(a);
    len2 = strlen(b);
    for(i=0;i<=len2;i++){

        a[len1+i] = b[i];
    }

    printf("%s",a);
    printf("%d",len1);
    printf("%d",len2);

    return 0;
}

# Write-a-program-that-prints-the-prime-numbers-in-the-range-1-to-n-with-n-integers-entered-from-the-
Write a program that prints the prime numbers in the range 1 to n, with n integers entered from the keyboard.
#include<stdio.h>
#include<conio.h>
main()
{
    int n,i,j,dem;
    printf("Nhap n="); 
    scanf("%d",&n);
    for(i=2;i<=n;i++)
    {        
        dem=0;
        for(j=2;j<=i/2;j++)
        {
            if(i%j==0)
            dem++;
        }        
        if(dem==0)
        {
            printf("%5d",i);
        }
    }
    getch();
}

# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Start
2.	Read an integer input n
3.	Repeat a loop from i = 0 to i < n:
4.	Inside the loop, print the number n
5.	After the loop ends, print a newline
6.	End

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    for(int i=0;i<n;i++){
        printf("%d ",n);
    }
    return 0;
}
```


## OUTPUT:


![image](https://github.com/user-attachments/assets/a02d5647-67a3-4a71-a258-67f7f5e59694)




## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Start
2.	Declare variables n, i, and j as integers.
3.	Read an integer n from the user (this will be the number of rows).
4.	Repeat the outer loop with variable i from 1 to n:
5.	For each i, repeat the inner loop with variable j from 1 to i:
6.	Print the character 'a' (without newline).
7.	After inner loop ends, print a newline (\n) to go to the next row.
8.	End


## PROGRAM:
```
#include <stdio.h>
int main(){
    int n,i,j;
    scanf("%d",&n);
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            
            printf("a");
        }
        printf("\n");
    }
}
```


## OUTPUT:

![image](https://github.com/user-attachments/assets/195030d5-ef73-4c2d-8f9d-45bae8dbbb7b)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Start
2.	Declare integers: n, i, sum = 0, t1 = 0, t2 = 1, and next.
3.	Read integer input n (number of Fibonacci terms to generate).
4.	Print the first two terms t1 and t2.
5.	Repeat a loop from i = 2 to i < n:
6.	Calculate next = t1 + t2
7.	Print next
8.	Add next to sum
9.	Update t1 = t2, t2 = next
10.	End the loop.
11.	End


## PROGRAM:
```
#include <stdio.h>
int main(){
    int i,n,sum=0;
    scanf("%d",&n);
    int t1=0,t2=1,next;
    printf("%d ",t1);
    printf("%d ",t2);
    for(i=2;i<n;i++)
    {
        next=t1+t2;
        printf("%d ",next);
        sum +=next;
        t1=t2;
        t2=next;
    }
    
    
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/09f9fcb7-3434-4751-8d10-072ed790ead2)


## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Start
2.	Input two integers: start and end (range bounds)
3.	Loop from num = start to end:
4.	Initialize sum = 0, temp = num
5.	While temp > 0:
6.	Get last digit: digit = temp % 10
7.	If digit is even (digit % 2 == 0), add to sum
8.	Remove last digit: temp /= 10
9.	Print the sum for num
10.	End

## PROGRAM:
```
#include <stdio.h>
int main(){
    int start, end, sum=0,num;
    scanf("%d",&start);
    scanf("%d",&end);
    num=start;
    while (num <= end){
        if(num%2==0){
            sum += num;
        }
        num++;
    }
    printf("%d",sum);
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/2a56a0a3-748d-4d31-b398-82b0f7f33ca6)


## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Write a C program to print rhombus  pattern

## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1. Start
2. Declare integers n, i, and j
3. Read integer n from the user (number of rows and number of 'A' characters in each row)
4. Loop i from 1 to n:
5. Loop j from n - i - 1 down to 0:
6. Print a space " " (to shift the row to the right)
7. Loop j from 1 to n:
8. Print 'A' (to form the rectangle)
9. Print a newline after each row
10. End



## PROGRAM:
```
#include <stdio.h>
int main(){
    int n,i,j;
    scanf("%d",&n);
    for(i=1;i<=n;i++)
    {
        for(j=n-i-1;j>=0;j--)
        {
            printf(" ");
        }
        for (j=1;j<=n;j++)
        {
            printf("A");
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/8ba8276e-f7ae-465a-b230-15c2d9a0247e)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 

# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<math.h>
void calc(float p, float r, float t) 
{
    float monthlyRate = r / (12 * 100);
    float totalMonths = t * 12;
    float amt = (p * monthlyRate * pow(1 + monthlyRate, totalMonths)) / (pow(1 + monthlyRate, totalMonths) - 1);
    printf("%.2f\n",amt);
}
int main() 
{
    float principal, rate, time;
    printf("Enter the principal amount, rate of interest and months: ");
    scanf("%f %f %f", &principal, &rate, &time);
    calc(principal, rate, time);
    return 0;
    
}
```

## OUTPUT
<img width="791" height="236" alt="image" src="https://github.com/user-attachments/assets/77bc8bc8-c2ea-4a69-8f57-813f6a704826" />





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main() 
{
    int n, n1=0, n2= 1,n3,i;
    scanf("%d",&n);
    for (i=1; i<=n;i++) 
    {
        printf("%d ", n1);
        n3=n1+n2;
        n1=n2;
        n2=n3;
    }
    return 0;
    
}
```
## OUTPUT
<img width="387" height="178" alt="image" src="https://github.com/user-attachments/assets/0099f1e0-5067-4d84-8c0c-cd5de6b54c17" />








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main() 
{
    int n;
    scanf("%d", &n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    printf("The last element is %d", arr[n-1]);
    return 0;
    
}
```
## OUTPUT
<img width="391" height="200" alt="image" src="https://github.com/user-attachments/assets/5407a3ac-bbef-4f84-a317-4f4ff209895b" />









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main() 
{
    int n,count=0;
    scanf("%d", &n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++)
    {
        if(arr[i]%2==0){
            count++;
        }
    }
    printf("%d",count);
    return 0;
    
}
```

## OUTPUT
<img width="382" height="206" alt="image" src="https://github.com/user-attachments/assets/90dc1601-a9eb-4c90-91d1-c3c11422b187" />





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include<stdio.h>
int main() 
{
    int n,count=0;
    scanf("%d", &n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    printf("The updated array after replacement:\n");
    for(int i=0;i<n;i++)
    {
        if(arr[i]%2==0){
            printf("E ");
        }
        else{
            printf("%d ",arr[i]);
        }
    }
    return 0;
    
}
```
## Output:
 <img width="420" height="256" alt="image" src="https://github.com/user-attachments/assets/5bf51c4a-668d-40fb-a8b5-ae67e108fc07" />



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




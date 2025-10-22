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
#include <stdio.h>
#include <math.h>
void calculateEMI(float p, float r, int t) {
    float emi;
    r = r / (12 * 100);
    emi = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
    printf("\nThe EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;
    printf("Enter the Principal amount: ");
    scanf("%f", &principal);
    printf("Enter the Annual Rate of Interest (in %%): ");
    scanf("%f", &rate);
    printf("Enter the Time in months: ");
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}

```
## OUTPUT
<img width="1622" height="737" alt="Screenshot 2025-10-22 101009" src="https://github.com/user-attachments/assets/8dc2403a-d887-4de1-a2c4-265e2898d036" />





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
#include <stdio.h>

int main() {
    int n = 6;
    int a = 0, b = 1, c, i;
    printf("Fibonacci Series for %d terms:\n", n);
    printf("%d %d ", a, b);
    for(i = 2; i < n; i++) {
        c = a + b;       
        printf("%d ", c);
        a = b;      
        b = c;
    }
    return 0;
}

```
## OUTPUT
<img width="1624" height="681" alt="Screenshot 2025-10-22 101235" src="https://github.com/user-attachments/assets/9fb9c778-09e7-4c47-81c2-c26ab53772ff" />


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
#include <stdio.h>
int main()
{
    int n;
    printf("Enter the number of element:");
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    printf("The last element of the array:%d",a[n-1]);
    return 0;
}
```
## OUTPUT
<img width="1615" height="680" alt="Screenshot 2025-10-22 101954" src="https://github.com/user-attachments/assets/a8b4db6d-7380-47d5-9ba8-92feecffeea0" />

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
#include <stdio.h>

int main() {
    int n, i, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++) {
        if(arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);
    return 0;
}

```

## OUTPUT
<img width="1616" height="728" alt="Screenshot 2025-10-22 103146" src="https://github.com/user-attachments/assets/bb6037bd-a00e-4e0a-896a-303534f22d68" />


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
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("\nArray after replacing even elements with 'E':\n");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    
    return 0;
}

```
## Output:
<img width="1616" height="769" alt="Screenshot 2025-10-22 103508" src="https://github.com/user-attachments/assets/a7541ff1-2765-49b0-8cf3-c41ce16dc102" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




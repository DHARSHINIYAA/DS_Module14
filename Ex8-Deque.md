# Ex8 Deque
## DATE:6.3.2025
## AIM:
To write a C function to count the number of elements present in the deque.

## Algorithm
1.Start the program.

2.Define a function count(arr) that takes an array arr as input.

3.Initialize a counter c = 0 to track the number of non-zero elements.

4.Loop through each element of the array from index 0 to MAX-1:
a. If the current element is not zero, increment the counter c.

5.After the loop ends, return the final value of c.

6.End the program.

## Program:
```
/*#include <stdio.h>
#define MAX 10
void addFront(int *, int, int *, int *);
void addRear(int *, int, int *, int *);
int delFront(int *, int *, int *);
int delRear(int *, int *, int *);
void display(int *);
int count(int *);
*/
int count(int *arr) {
int c = 0, i;
for(i=0;i<MAX;i++)
{
if(arr[i]!=0)
{
  c+=1
}
}
returnc;
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/8df12b02-893c-4213-b1a0-2c6f272e5324)


## Result:
Thus, the C code to count the number of elements present in the deque is implemented successfully.

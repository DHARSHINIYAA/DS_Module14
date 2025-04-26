# Ex9 Applications of Queue - SJF
## DATE: 6.3.2025
## AIM:
To incorporate the code to calculate the Total Waiting Time and Average Waiting Time in Shortest Job First scheduling algorithm.
## Algorithm
1.Start.

2.Read number of processes n and their burst times bt[].

3.Assign process numbers p[] from 1 to n.

4.Sort processes by burst time (adjust bt[] and p[] together).

5.Calculate waiting time wt[] and turnaround time tat[].

6.Compute and print average waiting time and turnaround time.

7.End.



## Program:
```
#include<stdio.h>
int main()
{
int bt[20],p[20],wt[20],tat[20],i,j,n,total=0,pos,temp;
float avg_wt,avg_tat;
scanf("%d",&n);
for(i=0;i<n;i++)
{
scanf("%d",&bt[i]);
p[i]=i+1;
}
for(i=0;i<n;i++)
{
pos=i;
for(j=i+1;j<n;j++)
{
if(bt[j]<bt[pos])
pos=j;
}
temp=bt[i];
bt[i]=bt[pos];
bt[pos]=temp;
temp=p[i];
p[i]=p[pos];
p[pos]=temp;
}
wt[0]=0;
for(i=1;i<n;i++)
{
wt[i]=0;
for(j=0;j<i;j++)
wt[i]+=bt[j];
total+=wt[i];
}
avg_wt=(float)total/n;
total=0;
printf("Process BurstTime WaitingTime TurnaroundTime\n");
for(i=0;i<n;i++)
{
tat[i]=bt[i]+wt[i]; //calculateturnaroundtime
total+=tat[i];
//printf("\n");
printf("p%d %d %d %d\n",p[i],bt[i],wt[i],tat[i]);
}
avg_tat=(float)total/n; //average turnaroundtime
//printf("\n");
printf("AverageWaitingTime=%f\n",avg_wt);
// printf("\n");
printf("AverageTurnaroundTime=%f\n",avg_tat);
return 0;
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/6883d4da-ece1-47aa-88d5-f10fd191db5b)


## Result:
Thus, the code to calculate the Total Waiting Time and Average Waiting Time in Shortest Job First scheduling algorithm is implemented successfully.

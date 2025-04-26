# Ex10 Applications of Queue – FCFS
## DATE:10.3.2025
## AIM:
To write a C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm.
## Algorithm
1.Start the program.

2.Initialize process[], burst_time[], and wait_time[] arrays.

3.Loop through each process from i = 0 to n-1.

4.For each process, compute tat[i] = burst_time[i] + wait_time[i].

5.End the program.
## Program:
```
nt turnaroundtime( int proc[], int n,int burst_time[], int wait_time[], int tat[]) {
 // calculating turnaround time by adding
 // burst_time[i] + wait_time[i]
 int i;
 for ( i = 0; i < n ; i++)
 tat[i] = burst_time[i] + wait_time[i];
 return 0;
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/b656f3a8-8c8a-46d6-8401-6b7817070a8a)


## Result:
Thus, the C function to calculate the turnaround time of each process given their burst time and waiting time in First Come first Serve scheduling algorithm is implemented successfully.

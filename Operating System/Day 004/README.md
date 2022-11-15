# Operating System

## CPU Scheduling Algorithms
There are various algorithms which are used by the Operating System to schedule the processes on the processor in an efficient way.

## Purpose of Scheduling Algorithms
* Maximum CPU utilization
* Fare allocation of CPU
* Maximum throughput
* Minimum turnaround time
* Minimum waiting time
* Minimum response time

## Algorithms

### First Come First Serve
It is the simplest algorithm to implement. The process with the minimal arrival time will get the CPU first. The lesser the arrival time, the sooner will the process gets the CPU. It is the non-preemptive type of scheduling.

### Round Robin
In the Round Robin scheduling algorithm, the OS defines a time quantum (slice). All the processes will get executed in the cyclic way. Each of the process will get the CPU for a small amount of time (called time quantum) and then get back to the ready queue to wait for its next turn. It is a preemptive type of scheduling.

### Shortest Job First
The job with the shortest burst time will get the CPU first. The lesser the burst time, the sooner will the process get the CPU. It is the non-preemptive type of scheduling.

### Shortest Remaining Time First
It is the preemptive form of SJF. In this algorithm, the OS schedules the Job according to the remaining time of the execution.

### Priority Scheduling
In this algorithm, the priority will be assigned to each of the processes. The higher the priority, the sooner will the process get the CPU. If the priority of the two processes is same then they will be scheduled according to their arrival time.

## Times Related to Process
### Arrival Time
The time at which the process enters into the ready queue is called the arrival time.

### Burst Time
The total amount of time required by the CPU to execute the whole process is called the Burst Time. This does not include the waiting time. It is confusing to calculate the execution time for a process even before executing it hence the scheduling problems based on the burst time cannot be implemented in reality.

### Completion Time
The Time at which the process enters into the completion state or the time at which the process completes its execution, is called completion time.

### Turnaround time
The total amount of time spent by the process from its arrival to its completion, is called Turnaround time.

### Waiting Time
The Total amount of time for which the process waits for the CPU to be assigned is called waiting time.

### Response Time
The difference between the arrival time and the time at which the process first gets the CPU is called Response Time.

# Operating System

## Process
A Program does nothing unless its instructions are executed by a CPU. A program in execution is called a process. In order to accomplish its task, process needs the computer resources.<br>
There may exist more than one process in the system which may require the same resource at the same time. Therefore, the operating system has to manage all the processes and the resources in a convenient and efficient way.<br>
The operating system is responsible for the following activities in connection with Process Management<br>
* Scheduling processes and threads on the CPUs.
* Creating and deleting both user and system processes.
* Suspending and resuming processes.
* Providing mechanisms for process synchronization.
* Providing mechanisms for process communication.

## Attributes of a Process
* Process ID
* Program Counter
* Process State
* Priority
* General Purpose Registers
* List of open files and devices

## Process States
![os-process-state-diagram](https://user-images.githubusercontent.com/114591698/201514948-2c7118bf-a2ce-4861-b37d-40e7fe4ff145.jpg)

## Process Schedulers
### 1. Long Term Scheduler:
Long term scheduler is also known as job scheduler. It chooses the processes from the pool (secondary memory) and keeps them in the ready queue maintained in the primary memory.<br>
Long Term scheduler mainly controls the degree of Multiprogramming. The purpose of long term scheduler is to choose a perfect mix of IO bound and CPU bound processes among the jobs present in the pool.
### 2. Short Term Scheduler:
Short term scheduler is also known as CPU scheduler. It selects one of the Jobs from the ready queue and dispatch to the CPU for the execution.<br>
A scheduling algorithm is used to select which job is going to be dispatched for the execution. The Job of the short term scheduler can be very critical in the sense that if it selects job whose CPU burst time is very high then all the jobs after that, will have to wait in the ready queue for a very long time.
### 3. Medium Term Scheduler:
Medium term scheduler takes care of the swapped out processes.If the running state processes needs some IO time for the completion then there is a need to change its state from running to waiting.<br>
Medium term scheduler is used for this purpose. It removes the process from the running state to make room for the other processes. Such processes are the swapped out processes and this procedure is called swapping. The medium term scheduler is responsible for suspending and resuming the processes.

## Process Queues
* Job Queue
* Ready Queue
* Waiting Queue

## Process Control Block
The Operating system maintains a process control block during the lifetime of the process. The Process control block is deleted when the process is terminated or killed. There is the following information which is saved in the process control block and is changing with the state of the process.<br>
![os-cpu-scheduling-process-control-block](https://user-images.githubusercontent.com/114591698/201515137-6506bea0-a80a-4dbb-9846-d32803904826.png)








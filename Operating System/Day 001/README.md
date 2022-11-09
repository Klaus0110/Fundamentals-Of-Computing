# Operating System
## Introduction
An Operating System can be defined as an interface between user and hardware. It is responsible for the execution of all the processes, Resource Allocation, CPU management, File Management and many other tasks.<br>
The purpose of an operating system is to provide an environment in which a user can execute programs in convenient and efficient manner.

## Tasks Of OS
* Process Management
* Process Synchronization
* Memory Management
* CPU Scheduling
* File Management
* Security of the System

## Structure of a Computer System
A computer system consists of:
* Users
* Application Programs
* System Programs
* Operating System
* Hardware

## Types Of OS
* **Batch OS**

In Batch operating system, access is given to more than one person; they submit their respective jobs to the system for the execution.<br>
The system put all of the jobs in a queue on the basis of first come first serve and then executes the jobs one by one. The users collect their respective output when all the jobs get executed.

* **Multiprogramming OS**

Multiprogramming is an extension to batch processing where the CPU is always kept busy. Each process needs two types of system time: CPU time and IO time.<br>
In a multiprogramming environment, when a process does its I/O, The CPU can start the execution of other processes. Therefore, multiprogramming improves the efficiency of the system.

* **Multiprocessing OS**

In Multiprocessing, Parallel computing is achieved. There are more than one processors present in the system which can execute more than one process at the same time. This will increase the throughput of the system.

* **Multitasking OS**

The multitasking operating system is a logical extension of a multiprogramming system that enables multiple programs simultaneously. It allows a user to perform more than one computer task at the same time.


* **Network OS**

An Operating system, which includes software and associated protocols to communicate with other computers via a network conveniently and cost-effectively, is called Network Operating System.

* **Real Time OS**

In Real-Time Systems, each job carries a certain deadline within which the job is supposed to be completed, otherwise, the huge loss will be there, or even if the result is produced, it will be completely useless.<br>
The Application of a Real-Time system exists in the case of military applications, if you want to drop a missile, then the missile is supposed to be dropped with a certain precision.

* **Time Sharing OS**

In time-sharing, the CPU is switched among multiple programs given by different users on a scheduled basis.<br>
Thus it helps to provide a large number of user's direct access to the main computer.

* **Distributed OS**

The Distributed Operating system is not installed on a single machine, it is divided into parts, and these parts are loaded on different machines. A part of the distributed Operating system is installed on each machine to make their communication possible.

## Operating System Structure
Operating system can be implemented with the help of various structures. The structure of the OS depends mainly on how the various common components of the operating system are interconnected and melded into the kernel. Depending on this we have following structures of the operating system:

* **Simple Structure**

Such operating systems do not have well defined structure and are small, simple and limited systems. The interfaces and levels of functionality are not well separated. MS-DOS is an example of such operating system. In MS-DOS application programs are able to access the basic I/O routines. These types of operating system cause the entire system to crash if one of the user programs fails.

![1](https://user-images.githubusercontent.com/114591698/200881079-f202e322-2e56-45b8-a5e9-2358d639a15a.png)

* **Layered Structure**

In this structure the OS is broken into number of layers (levels). The bottom layer (layer 0) is the hardware and the topmost layer (layer N) is the user interface. These layers are so designed that each layer uses the functions of the lower level layers only.<br>
This simplifies the debugging process as if lower level layers are debugged and an error occurs during debugging then the error must be on that layer only as the lower level layers have already been debugged.<br>

![2](https://user-images.githubusercontent.com/114591698/200881716-078cacb7-889e-4ac4-8ae3-64a61c4d1c86.png)

* **Micro-Kernel**

This structure designs the operating system by removing all non-essential components from the kernel and implementing them as system and user programs. This result in a smaller kernel called the micro-kernel.<br>
Advantages of this structure are that all new services need to be added to user space and does not require the kernel to be modified. Thus it is more secure and reliable as if a service fails then rest of the operating system remains untouched. Mac OS is an example of this type of OS.

* **Modular Structure**

It is considered as the best approach for an OS. It involves designing of a modular kernel. The kernel has only set of core components and other services are added as dynamically loadable modules to the kernel either during run time or boot time.<br>
It resembles layered structure due to the fact that each kernel has defined and protected interfaces but it is more flexible than the layered structure as a module can call any other module.<br>
For example Solaris OS is organized as shown in the figure.<br>

![3](https://user-images.githubusercontent.com/114591698/200882976-dac6ac16-bb23-4e46-b697-3d540bae1fc8.png)

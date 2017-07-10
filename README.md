# Operating Systems lab3

This is my lab 3 for Operating System Principles course in XMU. The assignment guide see [Nachos Project Guide] of V22.0202-001 in New York University.

In this lab, I implement an EventBarrier primitive and alarm clock primitive first. Then use them to solve Elevator problem.

## Installation
Now, you are in top directory. So, please enter into `threads` directory first.

```
cd threads
```

Compile the project.

```
make depend
make
```

Run the nachos. For the part 1 "Implementing an EventBarrier Primitive", you can use

```
./nachos -q 7 -t [num_threads]
```
where

- `-q 7`: test the EventBarrier
- `-t`: number of threads

For the part 2 "Implementing an Alarm Clock Primitive", you can use

```
./nachos -q 8 -t [num_threads]
```
where

- `-q 8`: test the Alarm
- `-t`: number of alarms

**BE CAREFUL!** Before you test the Alarm, please delete the comments in `system.cc` labeled with `*** ADDED *** in lab 3.2` first.

For the last part "Synchronization Problem 2: Elevator", you can use

```
./nachos -q 9 -t [num_threads] -F [num_floors] -E [num_elevators] -c [capacity]
```

Command line parameters are:

- `-q 9`: test the Elevator
- `-t`: number of riders
- `-F`: number of floors
- `-E`: number of elevators
- `-c`: capacity of a elevator

But, there exists **BUGS** when overloading occurs. Please **FIX** it!

## Acknowledgment
Dasong Chen, Jinbin Tan and Hao Dong assist me to finish this assignment. Thanks for their effort.

[Nachos Project Guide]: http://www.cs.nyu.edu/courses/spring05/V22.0202-001/nachos-labs.pdf
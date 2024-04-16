# Overview 
This project simulates the scheduling of processes with varying burst times using CPU scheduling algorithms including First Come First Serve (FCFS), Preemptive Shortest Job First (SJF), Round Robin, and Multilevel Feedback Queue (MLFQ). It serves as an interactive tool for individuals to learn and reinforce their understanding of process scheduling.

Users input the number of processes to simulate and specify burst times for each process. Processes, represented by structs and created via the fork() function, are stored in a dynamic array and passed into each algorithm.

## Features
- FCFS (First Come First Serve): Simulates process execution based solely on arrival times, requiring arrival time and burst time for each process.

- Preemptive Shortest Job First (SJF): Considers both arrival time and shortest burst time of processes. A process begins execution upon arrival unless a process with a shorter burst time arrives.

- Non-Preemptive Shortest Job First (SJF): Simulates process execution based solely on shortest burst times. Processes with shorter burst times are executed first.

- Round Robin: Allows users to specify a time quantum for simulation. Processes execute for the given quantum, and those not completing their burst time are enqueued for later execution.

- MLFQ (Multilevel Feedback Queue): Utilizes three queues: Q1 (round robin with time quantum 8), Q2 (round robin with time quantum 16), and Q3 (First Come First Serve). Processes run based on queue priority and move down queues as they exhaust time allotment. Processes in Q3 for 10 seconds are considered starving and moved to Q1. Preemptive arrival of processes prioritizes lower priority processes.

- Provides visualizations of scheduling results for each algorithm.
- Provides statistics such as total waiting time, total turnaround time, total response time, average waiting, and average turnaround time.

 ## Getting started
Processes created at the onset of the simulation traverse through all four scheduling algorithms implemented. 


- Navigate to the project directory 

- Make the script executable: chmod +x run_scheduler.sh 

- Run the simulation: ./run_scheduler.sh

 ## Link to YouTube Implementation Description Video
 https://youtu.be/2vBEym4XIPo

 ## Sample command-line visualization snippets: 
 ![WhatsApp Image 2024-04-16 at 23 10 05_bf2f8897](https://github.com/annaliesenartey/FinalProjectOS/assets/93687556/b8fc4b46-aab8-4f20-8555-7810e166078f)
 ![WhatsApp Image 2024-04-16 at 23 11 25_1cac65a5](https://github.com/annaliesenartey/FinalProjectOS/assets/93687556/9aabd152-7ff4-4102-a2e4-8f5360140726)

 
Project was implemented on Ubuntu 22.04  

Note: Program does not require web hosting and can be run locally.  



# Process Scheduling Simulation

## Overview
This program simulates various CPU scheduling algorithms to analyze their performance based on process burst time and arrival time. The program predicts the best scheduling algorithm for a given set of processes and computes the average waiting and turnaround times for each algorithm. It also generates a Gantt chart for visualization.

## Features
- **First-Come, First-Served (FCFS)**
- **Shortest Job First (SJF)**
- **Longest Job First (LJF)**
- **Shortest Remaining Time First (SRTF)**
- **Round Robin (RR)**

## Input Format
The program reads process data from an `input.txt` file. Each line in the file should contain:


## Output
The results are written to an `output.txt` file, including:
- Predicted best scheduling algorithm.
- Average waiting and turnaround times for each algorithm.
- Gantt chart representation for each algorithm.

## How to Use
1. **Compile the Program:**
   ```sh
   g++ -o scheduler scheduler.cpp

Run the Program:
./scheduler

Ensure the `input.txt` file is in the same directory as the executable and follows the specified format.

## Output
The results are written to an `output.txt` file. Check the `output.txt` file for the results.

## Scheduling Algorithms Explained
1. **First-Come, First-Served (FCFS):**
   - Processes are scheduled in the order they arrive.
   
2. **Shortest Job First (SJF):**
   - Processes with the shortest burst time are scheduled next.
   
3. **Longest Job First (LJF):**
   - Processes with the longest burst time are scheduled next.
   
4. **Shortest Remaining Time First (SRTF):**
   - Preemptive version of SJF. The process with the shortest remaining time is scheduled next.
   
5. **Round Robin (RR):**
   - Each process is assigned a fixed time quantum. Processes are scheduled in a cyclic manner.

## Predicting the Best Algorithm
The program predicts the best scheduling algorithm based on process burst times and arrival times using various heuristics, such as burst time variance and the proportion of long burst times.

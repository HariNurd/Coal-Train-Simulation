# Simulation of Coal Train Unloading Process with FIFO Approach and Crew Working Time Limitations

This repository contains the implementation of a simulation model designed to study the coal train unloading process at a facility, with particular attention to FIFO queuing and crew working time limitations. The project is part of a capstone project for the "Aplikasi Komputasi Matematika" course at the Department of Mathematics, IPB University.

## Project Overview

The unloading process for coal trains involves several complex variables, including the arrival times of trains, the duration of unloading, and the working hours of the crew. One of the key challenges in this process is "hogging out," which occurs when the crew reaches the end of their working hours before unloading is completed, requiring a replacement crew to be called in.

## Objectives

The main objectives of this project are:

- To simulate the coal train unloading process using the Julia programming language.

To calculate key statistics, including:
- Average and maximum time a train spends in the system.
- Proportion of time the unloading facility is busy, idle, or experiencing "hogging out."
- Average and maximum number of trains in the queue at any given time.
- Proportion of trains experiencing "hogging out" zero, one, or two times.

## Methodology

### Simulation Model

The simulation model is built using discrete event simulation techniques implemented in Julia. The simulation covers a period of 720 hours (30 days) and takes into account the following factors:
- Train Arrival: Trains arrive at the facility with independent, exponentially distributed intervals, averaging 10 hours.
- Unloading Time: The unloading time is uniformly distributed between 3.5 to 4.5 hours.
- Crew Work Time: Crews can work for up to 12 hours, after which they require replacement. The replacement crew arrival time is uniformly distributed between 2.5 to 3.5 hours.

### Key Features

- Discrete Event Simulation: The simulation models the system's state over time, capturing key events such as train arrivals, crew shift changes, and unloading operations.
- Julia Packages: Key packages used include ConcurrentSim for event simulation, Distributions for statistical functions, and ResumableFunctions for managing event-driven processes.

### Implementation

- Pseudocode Design: The simulation was first outlined in pseudocode to structure the program effectively.
- Julia Implementation: The model was implemented in Julia, leveraging its high performance for scientific computing.

### Output and Analysis

The simulation provides insights into the efficiency of the unloading process under varying conditions:
- Time Metrics: Average time spent by trains in the system, and the maximum time recorded during the simulation.
- Resource Utilization: The proportion of time the facility is busy, idle, or delayed due to "hogging out."
- Queue Statistics: Average and maximum length of the train queue.
- Hogging Out Events: Frequency of "hogging out" occurrences per train.

## License
This project is protected under the intellectual property regulations of IPB University. Unauthorized use, reproduction, or distribution of this material is prohibited without explicit permission from the authors and IPB University.

## Acknowledgements
This project was completed by Kelompok 3 as part of the Aplikasi Komputasi Matematika course at IPB University. We extend our gratitude to our instructors and peers for their support and feedback throughout this project.

# Double-Deck Elevator Simulation Analysis

## Overview

This repository presents a discrete-event simulation and performance analysis of a 26-floor double-deck elevator system under varying traffic conditions.

The study evaluates passenger flow behaviour, queue dynamics, machine utilisation, and system performance metrics during peak and off-peak scenarios.

---

## Objectives

- Model inbound and outbound passenger traffic
- Analyse queue and buffer performance
- Evaluate elevator utilisation
- Measure system KPIs (WIP, Avg Time, Sigma Rating)
- Compare performance under peak vs base conditions
- Assess dispatch logic efficiency

---

## System Model

The model includes:

- 26 Floors
- Top Deck & Bottom Deck elevators
- Call Point Queues (CallPointQ)
- Destination Buffers
- Loading & Unloading Decks
- Turnstile control
- Direction-change logic

Simulation logic flow was designed using structured rule-based event triggers.

---

## Data Inputs

Inbound and outbound traffic datasets were used to simulate real-world demand.

Example:
- Wednesday inbound traffic dataset
- Wednesday outbound traffic dataset

---

## Key Performance Indicators

- Average Waiting Time
- Maximum Waiting Time
- Work-in-Progress (WIP)
- Elevator Utilisation (% Busy vs % Idle)
- System Throughput
- Sigma Rating

---

## Results Summary

Base Model (19th Simulation Run):

- Total Entered: 480 passengers
- WIP: 20
- Average Time: 32.469
- Sigma Rating: 6.0

Peak Model (30th Simulation Run):

- Total Entered: 426 passengers
- WIP: 26
- Average Time: 33.139
- Sigma Rating: 6.0

---

## Key Insights

- Peak traffic significantly increased buffer congestion.
- UnloadingDeck showed high utilisation during peak periods.
- Direction-change logic influenced queue clearance efficiency.
- Double-deck configuration reduced the average wait compared to the single-deck baseline.

---

## Author

Hope Bukunmi Dada  
MSc. Engineering Project Management


docs/README.md

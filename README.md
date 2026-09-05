# 🚗 SimPy Car Wash Simulation

A discrete-event simulation of a car wash system developed using Python and SimPy.

## 📌 Project Overview

This project simulates a car wash system where cars arrive at random intervals and use a limited number of washing bays.

If all washing bays are busy, arriving cars must wait in a queue until a bay becomes available.

The simulation is used to analyze the performance of the system and compare different scenarios.

---

## 🎯 Objectives

The main objectives of this project are:

- Simulate a car wash system using discrete-event simulation
- Model random car arrivals
- Model limited washing resources
- Analyze customer waiting times
- Compare different numbers of washing bays
- Evaluate the impact of adding more resources

---

## ⚙️ Simulation Settings

| Parameter | Value |
|---|---:|
| Number of Cars | 12 |
| Mean Interarrival Time | 4 minutes |
| Minimum Wash Time | 6 minutes |
| Maximum Wash Time | 10 minutes |
| Random Seed | 42 |

---

## 🧩 Simulation Concepts

The project uses the following SimPy concepts:

- **Environment** → Manages the simulation time
- **Process** → Represents each car
- **Resource** → Represents the washing bays
- **Event / Timeout** → Represents waiting and washing time

---

## 🔄 System Flow

```text
Car Arrival
     ↓
Request Washing Bay
     ↓
Is a Bay Available?
   ↙        ↘
 Yes         No
  ↓           ↓
Wash Car    Wait in Queue
  ↓           ↓
Departure ←───

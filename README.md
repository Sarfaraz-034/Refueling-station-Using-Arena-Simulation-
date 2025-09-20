# Analysis of a Refueling Station using Arena Simulation
This project features a discrete-event simulation model of a vehicle refueling station, developed using Rockwell Arena. The primary objective is to analyze the performance of the station's servers and operators, evaluate operational costs, and understand the system's efficiency under varying conditions.


## 📝 Problem Statement
We are examining a refueling station equipped with three servers and three operators dedicated to refueling different types of vehicles: CNG, LPG, and Petrol. The management aims to evaluate the performance of these servers and understand the associated labor costs. Operator wages vary based on the station's activity, with a rate of 50 Taka/hour during busy periods and 30 Taka/hour during idle times. The simulation will provide insights into server utilization, customer wait times, and overall cost-effectiveness.

## 🎯 Project Objectives
Develop a Model: Construct a detailed simulation model of the refueling station system using Arena.
Simulate and Visualize: Run the simulation to visualize the flow of vehicles and the operation of the servers.
Analyze Performance: Measure and analyze the performance of the system by running the model for a specified number of replications.

## 📊 System Parameters & Distributions
The operational dynamics of the refueling station, including vehicle arrival rates and service times, are modeled using the following statistical distributions.


### Table 1: Distribution of Inter-Arrival Time (minutes)
Vehicle Type
Inter-Arrival Time Distribution
Vehicle_LPG
-0.001 + WEIB(0.484, 0.646)
Vehicle_CNG
-0.001 + WEIB(0.484, 0.646)
Vehicle_Petrol
-0.001 + WEIB(0.484, 0.646)

### Table 2: Distribution of Service Time (minutes)
Server
Service Time Distribution
Server 1
LOGN(2.91, 1.64)
Server 2
2 + EXPO(14.8)
Server 3
0.999 + EXPO(2.81)

## 🛠️ Model Details & System Logic
System Requirements: Windows OS and Rockwell Arena simulation software.
Entities: Vehicles (differentiated by type: LPG, CNG, and Petrol).
Resources: Operator 1, Operator 2, and Operator 3.
Processes: Server 1, Server 2, and Server 3.
Process Action: The core logic for the refueling service is Seize Delay Release.
Queue Discipline: The queuing system operates on a First-Come, First-Served (FCFS) basis.
z
## 🚀 How to Run the Simulation
Ensure you have Rockwell Arena installed on a Windows operating system.
Clone this repository or download the .doe model file.
Open the model file in Arena.
Set the desired number of replications to ensure statistical significance.
Execute the simulation to run the model and generate the output reports.
📈 Results & Analysis
The output from the Arena simulation will provide key performance indicators such as server utilization, average waiting times for each vehicle type, queue lengths, and total operational costs. This data is essential for identifying potential bottlenecks, optimizing resource allocation, and making informed decisions to improve the station's overall service and profitability.

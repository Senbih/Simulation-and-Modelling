# Simulation-and-Modelling
Modelling a bug tracking and Resolving system. 
Bug Tracking Simulation

Overview

This project simulates a bug tracking and resolution system using SimPy, a process-based discrete-event simulation framework. It models the process of assigning and resolving bugs by a team of developers and provides visual and statistical insights into system performance.

Features

Bug Assignment and Resolution: Bugs are assigned to developers based on availability, and resolution times are determined by priority and severity.

Developer Utilization Monitoring: Tracks and visualizes how efficiently the developer resources are utilized during the simulation.

Performance Analysis:

Average resolution time for bugs.

Resolution time distribution by bug priority.

Developer utilization over time.

Simulation Parameters

The simulation includes the following adjustable parameters:

NUM_DEVELOPERS: Number of developers available to resolve bugs.

ARRIVAL_RATE: Average rate of bug arrivals per unit time.

TOTAL_BUGS: Total number of bugs to simulate.

MONITOR_INTERVAL: Frequency (in time units) of developer utilization monitoring.

Prerequisites

Python 3.7+

Required libraries:

simpy

pandas

matplotlib

Install the libraries using pip:

pip install simpy pandas matplotlib

Usage

Clone the repository:

git clone https://github.com/yourusername/bug-tracking-simulation.git

Navigate to the project directory:

cd bug-tracking-simulation

Run the simulation:

python simulation.py

Code Description

Classes and Functions

BugTrackingSystem: Manages the developer pool, bug backlog, and bug resolution process.

bug_generator: Simulates the arrival of bugs with random priorities and severities.

assign_bug: Assigns bugs to available developers and initiates the resolution process.

monitor_utilization: Periodically tracks the number of active developers.

analyze_results: Analyzes and visualizes resolution times and other performance metrics.

plot_developer_utilization: Visualizes developer utilization over time.

Output

Console logs detailing bug assignments and resolutions.

Plots:

Bug resolution times.

Bug priority vs. resolution duration.

Developer utilization over time.

Experimentation

You can experiment with the following parameters:

Number of Developers (NUM_DEVELOPERS):

Increase or decrease the number of developers to observe changes in backlog and resolution times.

Bug Arrival Rate (ARRIVAL_RATE):

Simulate low or high bug arrival rates to evaluate system responsiveness.

Backlog Management Strategies:

Modify the bug assignment logic to prioritize critical bugs.

Example

Default parameters:

RANDOM_SEED = 42
NUM_DEVELOPERS = 5
ARRIVAL_RATE = 1.0
TOTAL_BUGS = 20
MONITOR_INTERVAL = 1  # Record utilization every 1 unit of time

Sample console output:

[2] Bug 0 assigned: Priority=4, Severity=2.50
[7] Bug 0 resolved
[7] Bug 1 assigned: Priority=2, Severity=1.80
[11] Bug 1 resolved
...

Generated plots:

Bug Resolution Times:


Developer Utilization Over Time:


Contributing

Feel free to fork this repository and contribute by submitting pull requests. Suggestions and bug reports are welcome.

License

This project is licensed under the MIT License.

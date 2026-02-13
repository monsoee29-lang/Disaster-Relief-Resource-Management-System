# Disaster Relief Resource Management System (Project Pathfinders 7.7)

A Data Structures and Algorithms Final Project 

Developed by: Ei Mon Soe & San San Maw

Course: Data Structures and Algorithms (Parami University)

**📌 Project Overview**

Following the catastrophic 7.7 magnitude earthquake in Myanmar on March 28, 2025, coordination of aid became a critical challenge. This project simulates an automated Disaster Relief Management System designed to optimize the logistics of donated resources.The application ensures that aid is not just distributed, but prioritized based on the severity of the disaster and the most efficient travel routes.

**🛠 Data Science & Algorithmic Workflow1.**

**(1) Data Structures for Logistics**

To manage the flow of resources, we implemented three core data structures:

- Singly Linked List (Donation Management): Used to track incoming donations from NGOs and individuals. This allows for $O(1)$ time complexity when adding new donations to the front of the registry.

- Priority Queue (Crisis Prioritization): Disaster reports are handled using a Priority Queue. This ensures that a "Level 1" urgency (Critical) is always processed before a "Level 5" (Minor), regardless of which report was received first.

- Graph Theory (Logistics Networking): The regions are represented as a weighted graph where nodes are cities (Yangon, Mandalay, etc.) and edges are the travel distances between them.

**(2) Algorithmic Implementation**

- Dijkstra’s Algorithm: We implemented Dijkstra’s algorithm to find the Shortest Path from a central storehouse to a disaster-stricken location. This minimizes delivery time, which is life-saving in a 7.7 magnitude earthquake scenario.

- Error Handling: The system includes robust input validation to handle missing data, non-numeric urgency levels, and out-of-range values.Shutterstock3.

**(3) Performance & Complexity Analysis**

We conducted a time complexity analysis to ensure the system remains scalable during high-volume disaster events:

- Append Donations: $O(n)$

- Priority Dispatching: $O(\log n)$

- Shortest Path Calculation: $O(V^2)$ (using a standard Dijkstra implementation, where $V$ is the number of locations).

**🚀 Key Features**

Real-time Reporting: Users can report disasters with urgency levels (1-5).

Automated Matching: The system matches the most urgent aid request with the next available donation in the Linked List.

Interactive Menu: A CLI (Command Line Interface) allows users to manage donations, view supplies, and calculate the fastest routes instantly.

Pathfinding: Instant calculation of distances from a starting point to all reachable disaster zones.

**📊 Technical Stack**

- Language: Python 3.x

- Core Libraries: queue (PriorityQueue), time, json

- Environment: Developed and tested on Google Colab

**Report**

https://docs.google.com/document/d/1UsoG1LKsVzQS7FSW8i8UoMxdbLy4AMR856uLF7rtJ4k/edit?usp=sharing








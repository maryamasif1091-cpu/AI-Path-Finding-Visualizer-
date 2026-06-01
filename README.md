# 🧭 Dynamic Pathfinding Agent

## 📌 Project Overview
This project implements a **Dynamic Pathfinding Agent** that navigates a grid-based environment using informed search algorithms.

The agent finds a path from a **Start Node** to a **Goal Node** using:
-  A* Search  
-  Greedy Best-First Search (GBFS)

The application visualizes:
- Visited nodes
- Frontier nodes
- Final optimal path
- Real-time performance metrics

---

## ✨ Features
-  Dynamic grid sizing (user-defined rows and columns)
-  Start and goal node selection
-  Random obstacle generation with adjustable density
-  Interactive map editor (add/remove walls)
-  Two heuristic functions:
  - Manhattan Distance
  - Euclidean Distance
-  Step-by-step visualization of search process
-  Real-time metrics dashboard:
  - Nodes visited
  - Path cost
  - Execution time

---

## 🧮 Algorithms Implemented

###  1. A* Search
Uses the evaluation function:

f(n) = g(n) + h(n)

Where:
- g(n): cost from start node  
- h(n): heuristic estimate to goal  

---

###  2. Greedy Best-First Search (GBFS)
Uses:

f(n) = h(n)

This algorithm selects nodes purely based on heuristic value.

---

## 📐 Heuristics

###  Manhattan Distance
|x1 - x2| + |y1 - y2|

###  Euclidean Distance
√((x1 - x2)² + (y1 - y2)²)

---

## 🛠️ Technologies Used
-  Python
-  Tkinter (GUI)
-  Jupyter Notebook

---

## ⚙️ Installation

1. Install Python (3.8 or higher recommended).

2. Install required libraries (if needed):
```bash
pip install tkinter
```

> Note: Tkinter is usually pre-installed with Python.

---

## 🚀 How to Run

###  Option 1: Jupyter Notebook
1. Open Jupyter Notebook
2. Load the project notebook file
3. Run all cells
4. Provide inputs:
   - Grid rows 
   - Grid columns 
   - Obstacle density 
   - Algorithm (A or G)
   - Heuristic (M or E)

GUI will launch automatically.

---

###  Option 2: Python Script
```bash
python main.py
```

Then follow terminal prompts.

---

## 🎮 GUI Controls

-  Start Mode → Set start node  
-  Goal Mode → Set goal node  
-  Wall Mode → Add obstacles  
-  Random → Generate random obstacles  
-  Start Search → Run algorithm  
-  Clear → Remove all obstacles  
-  Reset → Reset visualization  

---

## 🎨 Visualization Details

The GUI highlights:
- 🟡 Frontier Nodes (in queue)
- 🔵 Visited Nodes (already explored)
- 🟩 Final Path (optimal route)

It also displays:
-  Total nodes visited
-  Path cost
-  Execution time
 

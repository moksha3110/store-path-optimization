# 🛒 Store Path Optimization App

This is a **Python application** built using **Streamlit** that helps users find the **optimal path through a store** based on their shopping list.  
The app computes the most efficient route to navigate from the **entrance** to the **billing counter**, ensuring all selected items are picked up along the way.

---

## 🎯 Aim

The goal of this project is to **minimize the time and distance** shoppers spend in the store.  
By mapping out the store layout and computing the **shortest path** through all required sections, the app optimizes the shopping experience — making it faster, easier, and more convenient.

---

## ⚙️ Approach

### 1. **Graph Representation**
- The store layout is modeled as a **directed weighted graph** using the `NetworkX` library.  
- Each **node** represents a store section (e.g., *Produce*, *Bakery*, etc.).  
- Each **edge** represents a path between sections, with **weights** corresponding to the distance between them.

### 2. **Optimal Path Calculation**
- A **greedy algorithm** is used to compute a near-optimal path.
- The path starts at the **Entrance**, iteratively visits the nearest required section from the current position, and ends at the **Billing Counter**.
- The final route includes the **shortest paths** between all relevant nodes.

### 3. **Graph Visualization**
- The store layout and optimal path are visualized using **Matplotlib**.
- Nodes are color-coded:
  - 🟢 Shopping list items  
  - 🔴 Entrance and Billing Counter  
- Users can view the **entire graph**, or reveal the path step-by-step to understand the sequence of visits.

---

## 🌟 Features

✅ **User-friendly Interface** – Built with Streamlit for simple, interactive use.  
✅ **Interactive Path Display** – Step-by-step visualization of the optimal route.  
✅ **Graph Visualization** – Clear and intuitive display of the store layout and connections.  
✅ **Custom Shopping Lists** – Users can dynamically select their own list of items.  

---

## 🧩 Tech Stack

- **Python 3.x**
- **Streamlit**
- **NetworkX**
- **Matplotlib**

---



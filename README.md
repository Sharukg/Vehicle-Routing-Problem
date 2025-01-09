# 🚚 Vehicle Routing Optimizer 🗺️

This project implements a **Vehicle Routing Problem (VRP)** optimizer using a **Genetic Algorithm (GA)**. The optimizer determines the most efficient routes for a fleet of vehicles starting and ending at a central depot to visit a set of locations.

---

## ✨ Features

- 🔄 **Flexible Inputs**: Configure the number of locations and vehicles.
- 🧬 **Genetic Algorithm**: Includes crossover, mutation, and selection operators tailored for routing optimization.
- 📊 **Fitness Function**: Minimizes the total distance traveled while balancing the routes across vehicles.
- 🖼️ **Visualization**: Plots the optimized routes for easy interpretation.

---

## 📦 Prerequisites

### 📚 Libraries
Make sure the following libraries are installed in your environment:

- `matplotlib` 📉
- `deap` 🧬
- `numpy` 🔢

Install them using:
```bash
pip install matplotlib deap numpy
```

---

## 🚀 Project Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-folder>
```

2. Open the project in your preferred editor (e.g., VSCode ✏️).

3. Run the main Python script:
```bash
python main.py
```

---

## 🛠️ Code Breakdown

### 1. 🗺️ Problem Setup
- Define the number of locations and vehicles.
- Generate random coordinates for the locations and depot.

### 2. 🧬 Genetic Algorithm
- **Encoding**: Represents routes as permutations of location indices.
- **Operators**: Uses Order Crossover (OX), Swap Mutation, and Tournament Selection.
- **Fitness Function**: Evaluates the total distance and route balance.

### 3. 🖼️ Visualization
- A `plot_routes` function plots the depot, locations, and routes for each vehicle using `matplotlib`.

---

## 🎯 Example Output

### Parameters
- **Locations**: 10 📍
- **Vehicles**: 3 🚚
- **Depot**: (50, 50) 🏠

### Visualization
Optimized routes:

- 🚚 Vehicle 1 (Blue)
- 🚚 Vehicle 2 (Green)
- 🚚 Vehicle 3 (Orange)

![Example Plot](example_plot.png)

---

## 🧩 How It Works

1. **Initialization**:
   - Generate an initial population of route permutations.
2. **Evaluation**:
   - Compute fitness (total distance, standard deviation of routes).
3. **Evolution**:
   - Apply crossover, mutation, and selection to improve solutions.
4. **Termination**:
   - Stop after a fixed number of generations or when no significant improvement is observed.

---

## 🔮 Future Enhancements
- Add vehicle capacity constraints.
- Optimize for other objectives (e.g., fuel efficiency 🌿).
- Include real-world location data 🌎.

---

## 🤝 Contributing
Feel free to fork this repository, add features, and create pull requests! 🎉

---

## 📜 License
This project is licensed under the MIT License. See the `LICENSE` file for details.

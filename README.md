### **Project Overview: Schelling's Dynamic Models of Segregation**

This project simulates Thomas Schelling's *Dynamic Models of Segregation* using agent-based modeling principles. The primary goal is to explore how simple individual preferences for neighbors of the same type can lead to large-scale patterns of segregation, even in cases where those preferences are not extreme. 

We start with a simple, basic version of the model (Version 1, the "skateboard") and progressively build toward a more complex and context-aware version (the "car"). Along the way, we incorporate additional features, such as richer agent decision-making processes and environmental contexts, using tools like the **Expected Parrot Digital Twin Framework (EDSL)** to simulate agent interactions and qualitative data collection.

---

### **High-Level Goals:**

1. **Understanding Segregation**: 
   - Model how local preferences can lead to large-scale segregation, and study different parameters that influence segregation patterns.
   
2. **Progressive Model Complexity**:
   - Develop multiple versions of the simulation, starting from a basic agent-based model and advancing to a more sophisticated one with complex agents, contextual data, and qualitative output.
   
3. **Integration with EDSL**:
   - Use EDSL to add context to agents and environments, allowing for richer simulations where agents have memory, emotional states, and can log qualitative experiences.

---

### **Project Structure**

The repository is organized into multiple folders to reflect the different versions and stages of development, from the initial simple model to the more complex EDSL-driven simulation.

#### **Directory Structure:**

```
/Schelling-Segregation-Simulation/
│
├── README.md                # Main project description and setup instructions
├── requirements.txt          # List of dependencies for the project
├── LICENSE                   # License for the project
│
├── /version_1_skateboard/    # Basic model with minimal complexity
│   ├── segregation_model.py  # Python script for Version 1 (basic functionality)
│   └── README.md             # Description and instructions for Version 1
│
├── /version_2_bicycle/       # Enhanced model with improved movement and weighted preferences
│   ├── segregation_model.py  # Python script for Version 2
│   └── README.md             # Description and instructions for Version 2
│
├── /version_3_motorcycle/    # Complex agents and grid with dynamic interactions
│   ├── segregation_model.py  # Python script for Version 3
│   └── README.md             # Description and instructions for Version 3
│
├── /version_4_car/           # Final version with EDSL integration, qualitative data collection
│   ├── segregation_model.py  # Python script for Version 4
│   ├── edsl_integration.py   # Additional integration for EDSL-driven contextual simulation
│   └── README.md             # Description and instructions for Version 4
│
└── /docs/                    # Documentation and explanation of the project
    ├── overview.md           # General project overview and background on Schelling's model
    ├── edsl_integration.md   # Documentation on how EDSL is integrated into the model
    └── versions.md           # Explanation of the different versions and their features
```

---

### **Key Components of the Project:**

1. **Agents**: 
   - Each agent has basic preferences regarding their neighbors and makes decisions about moving based on satisfaction with their current environment. In later versions, agents are enriched with contextual data, like emotions and memory of past moves.

2. **Grid/Environment**:
   - The grid serves as the environment in which agents are placed. In early versions, it's a simple 2D grid, but in later versions, it becomes more dynamic with location-based factors that influence agent decisions.

3. **Simulation**:
   - The main simulation runs a series of iterations where agents assess their satisfaction and move if necessary. As we progress through versions, the simulation becomes more complex, with richer data collected and more sophisticated movement algorithms.

4. **EDSL Integration**:
   - In the final stages of the project, we incorporate EDSL to add narrative-driven agent behavior and contextual analysis, making the simulation more reflective of real-world dynamics and producing qualitative as well as quantitative results.

---

### **Future Directions**:
- **Advanced Metrics**: Adding more advanced metrics to measure segregation (e.g., entropy, clustering coefficients).
- **Real-World Data**: Integrating real-world data to simulate actual neighborhoods, potentially for policy analysis.
- **Visualizations**: Developing graphical tools to visualize agent movements, neighborhood changes, and segregation dynamics over time.

---

### **Getting Started**:

1. **Clone the Repo**:
   ```bash
   git clone https://github.com/username/Schelling-Segregation-Simulation.git
   cd Schelling-Segregation-Simulation
   ```

2. **Install Dependencies**:
   - You can install the required Python packages via `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Basic Model (Version 1)**:
   - Navigate to the `version_1_skateboard` directory and run the model:
   ```bash
   cd version_1_skateboard
   python segregation_model.py
   ```

4. **Explore More Complex Models**:
   - As the project progresses, you can explore more advanced versions in the corresponding directories (`version_2_bicycle`, `version_3_motorcycle`, etc.).

---

### **Contributing**:

We welcome contributions! To contribute to this project:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

---

This setup will help manage the increasing complexity of the project as we move from a simple agent-based model to a more contextually rich simulation with EDSL. Each version builds on the previous one, adding new features and complexity in a structured way.

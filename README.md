# AEGIS
##  Overview

AEGIS is an innovative Unity-based space game that demonstrates advanced artificial intelligence through reinforcement learning. The project features autonomous spacecraft navigation using ONNX models derived from custom-trained RL algorithms, showcasing real-time space weather data integration, dynamic pathfinding, and intelligent decision-making systems.

### Training Pipeline

The RL models are trained using **PPO (Proximal Policy Optimization)** with curriculum learning:

```python
# Curriculum Stages
1. Easy Mode: No obstacles, basic navigation
2. Medium Mode: Static obstacles, moderate complexity  
3. Hard Mode: Dynamic obstacles, crisis scenarios
```
### Model Architecture

## Model Visualizations

This section showcases the visual representations and architecture diagrams of our AI models:

---

### Training Progress & Performance Metrics
![ODIN's Safest Mode Trajectory (High Fuel Budget)](images/1.jpg)  
*Shows ODIN executing a safe but fuel-heavy avoidance maneuver around a dense risk zone.*

![ODIN's Explorer Mode Trajectory (Low Fuel Budget)](images/2.jpg)  
*Depicts ODIN conserving fuel by taking a riskier but efficient trajectory.*

![A* Path Planning for a Static Obstacle](images/3.jpg)  
*Demonstrates basic A* algorithm navigating around a simple static hazard.*

---

### Model Architecture Diagrams

![Overall System Architecture and Training Process](images/16.jpg)  
*High-level ODIN workflow showing multi-stage RL training and system components.*

![Meteor Specific Curriculum](images/12.jpg)
*The model learns to make small maneuvers around the meteor objects.*

---

### ONNX Model Visualization
![Dynamic Risk Map Forecasting](images/7.jpg)  
*Left: current risk map (T=0). Right: forecasted risk map (T+30 min), enabling proactive avoidance.*

![Proactive Avoidance of Forecasted Hazard](images/8.jpg)  
*ODIN begins avoidance well before a hazard reaches its future predicted position.*

---

### Agent Behavior Examples
![Safe vs. Explorer Routing Strategies](images/6.jpg)  
*Heatmap contrasting conservative vs. aggressive routing strategies.*

![Learned Avoidance Maneuver (Tight Skim)](images/4.jpg)  
*ODIN agent performing a smooth, fuel-efficient avoidance path close to a wall hazard.*

![Learned Avoidance Maneuver (Wide Arc)](images/5.jpg)  
*ODIN agent executing a wider, safer avoidance arc around the same hazard.*

# AI-Based Traffic Optimization Simulation  
## Case Study: Kami-Shakujii Railroad Crossing Congestion

This project simulates traffic congestion and bus delay　around the railroad crossing near Kami-Shakujii Station in Tokyo.

The goal is to evaluate whether AI-based traffic control and routing optimization can reduce congestion and improve bus punctuality during the morning rush hour.

---

## Background

The area around Kami-Shakujii Station experiences severe traffic congestion during the morning rush hour due to several structural factors:

- Narrow road infrastructure
- High bus traffic
- Significant private vehicle traffic
- A frequently closed railroad crossing
- Many bus routes must cross the railroad

During peak hours, the railroad crossing remains closed for a large portion of time due to frequent train operations, causing vehicle queues and bus delays.

---

## Research Objective

This project evaluates the potential impact of two proposed improvements:

1. **AI-based vehicle routing**
   - Private vehicles are dynamically redirected to alternative routes to distribute traffic.

2. **Autonomous bus operation with real-time traffic awareness**
   - Bus movement is optimized based on traffic flow and railroad crossing conditions.

The goal is to measure how these strategies affect:

- Bus delays
- Traffic congestion
- Sensitivity to railroad crossing closure rates

---

## Simulation Overview

The simulation models the following components:

- Railroad crossing open/close cycles derived from train schedules
- Vehicle arrivals modeled as stochastic traffic flow
- Queue formation at the railroad crossing
- Bus movement and delay accumulation
- AI-based traffic control strategies

Monte Carlo simulations are used to account for variability in traffic conditions.

---

## Repository Structure


kamishakujii-traffic-simulation/

src/
traffic_simulation_v2.py
sensitivity_analysis.py

data/
railroad_crossing_schedule.csv

results/

docs/


---

## How to Run

Install Python dependencies:


pip install -r requirements.txt


Run the main simulation:


python src/traffic_simulation_v2.py


Run the sensitivity analysis:


python src/sensitivity_analysis.py


---

## Sensitivity Analysis

Sensitivity analysis evaluates how changes in the railroad crossing closure rate affect bus delays.

Tested closure rates:

- 70%
- 75%
- 80%
- 85%

This analysis helps determine how robust the proposed traffic optimization strategy is under different train traffic conditions.

---

## Key Metrics

The simulation evaluates:

- Average bus delay
- Maximum bus delay
- Total bus delay
- Traffic queue length
- Congestion levels

---

## Technologies Used

- Python
- NumPy
- Matplotlib

---

## Future Work

Possible extensions include:

- Real-world traffic sensor data integration
- Reinforcement learning traffic control
- Multi-intersection traffic modeling
- Real-time bus scheduling optimization

---

## License

This project is released under the MIT License.

---

## Author

Traffic simulation study for evaluating AI-based congestion mitigation strategies near Kami-Shakujii Station.

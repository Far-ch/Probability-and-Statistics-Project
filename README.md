# Engineering Probability and Statistics: Queuing Theory & Edge Computing

This repository contains the complete two-phase project for the "Engineering Probability and Statistics" course at Sharif University of Technology. The project explores the mathematical foundations of Queuing Theory and its practical application in modeling and simulating Edge Computing systems.

---

## 🎓 Project Metadata
* **Institution:** Sharif University of Technology, Department of Electrical Engineering
* **Instructor:** Dr. Mohammad Mahdi Mojahedian
* **Authors:** Farnoosh Chogani 
* **Timeline:** Fall 2024 – Winter 2025

---

## 📘 Phase 1: Foundations of Queuing Theory
Phase 1 focuses on the theoretical derivation of stochastic processes and performance metrics essential for understanding system behavior.

### Key Topics Covered:
* **Performance Metrics:** Analysis of System Utilization ($\rho = \lambda/\mu$), Little’s Law ($L = \lambda W$), and throughput bounds.
* **Stochastic Distributions:** Mathematical proofs regarding the Memoryless property of the Exponential distribution and the behavior of Poisson processes (merging and splitting).
* **Markov Chains:** Derivation of steady-state distributions ($\pi$) and balance equations (Rate In = Rate Out) for stable systems.
* **Order Statistics:** Analyzing the expected values of minimum/maximum service times across multiple parallel servers.



---

## 💻 Phase 2: Edge Computing System Simulation
Phase 2 applies the theoretical concepts from Phase 1 to model a real-world Edge Computing environment, focusing on task processing, buffer limits, and cost optimization.

### Key Components:
* **System Modeling:** * **Arrivals:** Modeled as a Poisson process with rate $\lambda$.
    * **Service:** Modeled with an Exponential distribution with rate $\mu$.
    * **Buffer Management:** Analysis of **M/M/1/K** systems where tasks are dropped once the finite buffer capacity ($K$) is reached.
* **Simulation (Python):** * Discrete-event simulation to monitor queue lengths over time.
    * Comparison of transient states vs. steady-state performance.
    * Analysis of job drop rates across different utilization levels ($\rho$ ranging from 0.05 to 2.0).
* **Cost Optimization:** * Evaluation of a cost function $C = A \cdot R_{drop} + B \cdot R_{return}$.
    * Mathematical determination of the optimal $\mu$ and buffer strategy based on the weight of penalty $A$ (task loss) vs. $B$ (task return).



---

## 📂 Repository Structure
```text
├── Phase 1/               
│   └── PS_Project_Phase1.pdf    # Final report for Phase 1
├── Phase 2/
│   ├── Phase 2.ipynb            # Jupyter Notebook with Python simulation
│   └── Project_Phase2.pdf       # Technical report for Phase 2


### GPU-Accelerated Particle Simulation & Visualization in Unreal Engine 5

**Lorenz Simulation** is a real-time GPU-accelerated simulation and visualization project developed using **Unreal Engine 5.8 and C++**.

The project focuses on simulating the Lorenz attractor system through numerical integration and visualizing its dynamic behavior using a custom GPU-based particle rendering pipeline.

The goal is to explore high-performance scientific visualization within Unreal Engine, combining mathematical simulation, GPU computation, and real-time graphics.

![Lorenz Simulation Overview](https://github.com/arvin-chamasemani/LorenzSimulation/tree/main/media/LorenzSimulation.gif)

## Project Features

- **GPU-Accelerated Simulation:** Particle state calculations performed on the GPU.
- **RK4 Numerical Integration:** Runge–Kutta fourth-order integration for solving the Lorenz differential equations.
- **Real-Time Visualization:** Custom particle rendering pipeline integrated into Unreal Engine.
- **Configurable Parameters:** Lorenz system parameters Sigma, Rho, and Beta.
- **Particle Visualization:** Custom particle appearance, color gradients, opacity, and size controls.
- **Unreal Engine Integration:** Developed as a modular Unreal Engine plugin.
  
![Simulation Parameters](https://github.com/arvin-chamasemani/LorenzSimulation/blob/main/media/LorenzSimulation.mp4)

## Technology Stack

| Technology | Purpose |
|---|---|
| Unreal Engine 5.8 | Real-time simulation and visualization |
| C++ | Plugin architecture and simulation management |
| HLSL / Unreal Shaders | GPU computation and particle rendering |
| DirectX 12 | Target graphics backend |
| Render Dependency Graph (RDG) | GPU resource and compute-pass management |

## Mathematical Model

The simulation is based on the Lorenz system, a set of three coupled nonlinear differential equations that describe chaotic dynamical behavior.

The governing equations are:

```text
dx/dt = Sigma * (y - x)

dy/dt = x * (Rho - z) - y

dz/dt = x * y - Beta * z
```

### System Parameters

- **x, y, z:** State variables describing the particle position.
- **Sigma:** Prandtl number.
- **Rho:** Rayleigh number.
- **Beta:** Geometric parameter.

The system is numerically integrated using the **fourth-order Runge–Kutta (RK4) method** to calculate particle trajectories over time.

This numerical approach enables real-time GPU-based simulation and visualization of the Lorenz attractor in Unreal Engine 5.
## Architecture Overview

The project consists of three primary systems:

1. **Simulation System:** Calculates particle trajectories using RK4 integration.
2. **GPU Resource Management:** Manages particle state buffers and simulation updates.
3. **Rendering System:** Visualizes the resulting particle positions in Unreal Engine.

## Platform

- Unreal Engine 5.8
- Windows
- DirectX 12
- NVIDIA RTX-class GPU recommended

## Distribution

The complete plugin is intended for distribution through **Fab**.

This GitHub repository serves as the project's public overview and documentation. It does not contain the plugin's implementation source code.

**Marketplace:** Coming soon.

---

*Developed as an independent GPU simulation and real-time visualization project.*

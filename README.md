# 📦 AI-Powered 3D Bin Packing System

An end-to-end ecosystem designed to solve the **3D Bin Packing Problem (3D-BPP)** using Deep Reinforcement Learning. This system optimizes the placement of boxes within containers to maximize volume utilization, ensuring physical stability and valid rotations.

---

## 🛰️ System Architecture

This project is organized into specialized repositories, linked here as **Git Submodules** to maintain a clean separation of concerns:

| Component | Description | Tech Stack | Repository |
|-----------|-------------|------------|------------|
| **AI Training** | Environment simulation and RL model training (DQN/PPO). | Python, Gym, SB3 | [Explore](https://github.com/alvaro-frank/3d-bpp) |
| **Backend API** | High-performance inference service using Clean Architecture. | FastAPI, ONNX, Pytest | [Explore](https://github.com/alvaro-frank/3d-bpp-backend) |
| **Frontend UI** | *[Planned]* Interactive 3D visualization dashboard. | React, Three.js, TS | [TBD] |



---

## 🛠️ Key Features

- **Physics-Aware Packing**: Implements **Action Masking** and heightmaps to prevent box overlapping or out-of-bounds placements.
- **Production-Ready Inference**: Models are exported to **ONNX** for fast execution without the overhead of heavy DL frameworks.
- **Strict Domain Logic**: Core business rules are decoupled from the infrastructure, following Clean Architecture.
- **Automated Quality**: Integrated CI/CD pipelines for automated testing and Docker image builds.

---

## ⚡ Quick Start

To run the current stable version of the backend service:

1. **Clone the Master Repository with Submodules**:
```bash
git clone --recursive [https://github.com/alvaro-frank/3d-bpp-system.git](https://github.com/alvaro-frank/3d-bpp-system.git)
cd 3d-bpp-system
```

2. **Launch via Docker Compose**:
```bash
docker-compose up --build
```

3. **Access API Documentation**:

Visit `http://localhost:8000/docs` to test the endpoints.

Developed by Álvaro Franco - [LinkedIn](https://www.linkedin.com/in/alvaro-jose-franco/)

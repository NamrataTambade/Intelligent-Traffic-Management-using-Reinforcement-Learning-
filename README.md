# 🛣️ Intelligent Traffic Management using Reinforcement Learning (DQN + SUMO)

This project uses **Deep Q-Learning (DQN)** and the **SUMO traffic simulator** to intelligently control traffic lights in a simulated city. The goal is to **reduce congestion**, **minimize vehicle wait times**, and **improve traffic flow** using AI-based decisions.

---

## 📌 Project Overview

Traditional traffic signals operate on fixed timers, often leading to unnecessary delays. Our project introduces **AI-controlled signals** that adapt to real-time traffic conditions using **Reinforcement Learning (RL)**.

We use:
- **SUMO (Simulation of Urban MObility)** to simulate traffic
- **OpenAI Gym-like environment** to interface SUMO with Python
- **DQN Agent** (Deep Q-Learning) for learning optimal traffic light actions

---

## 🧠 Tech Stack

| Component           | Technology                     |
|--------------------|---------------------------------|
| Simulation         | SUMO (sumo, sumo-gui)           |
| AI Agent           | Deep Q-Learning (DQN)           |
| Programming        | Python 3.8+                     |
| Libraries          | TensorFlow or PyTorch, NumPy    |
| Interface          | TraCI (SUMO <--> Python bridge) |
| Visualization      | Matplotlib / logs (optional)    |

---

## 📁 Project Structure

intelligent-traffic-rl/
│
├── dqn_agent.py # Deep Q-Learning agent
├── train.py # Main training loop
├── test.py # Model testing script
├── traffic_env.py # SUMO traffic simulation as RL environment
│
├── sumo_config/ # SUMO network & route files
│ ├── map.net.xml
│ ├── route.rou.xml
│ ├── traffic.sumocfg
│
├── models/ # Trained model weights
├── logs/ # Training logs & plots
├── requirements.txt # Python dependencies
├── README.md # Project overview & instructions
└── run.sh # Shell script to run training

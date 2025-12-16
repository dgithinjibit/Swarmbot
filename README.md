# 🤖 Project Chimera: Decentralized AI Sniper Swarm Simulation (Unity/ZetaChain/MeTTa)

> **Disclaimer:** This project is a purely **open-source, academic simulation** designed to explore the convergence of decentralized networking (Web3), reinforcement learning, and symbolic AI reasoning within a physics-based environment (Unity). It is **not** intended for actual military or defense applications.

## 🌟 Overview

Project Chimera is a cutting-edge simulation built in Unity that demonstrates a swarm of AI-powered sniper bots capable of learning, communicating, and executing complex missions within a simulated environment. The core innovation lies in the integration of three key technologies:

1.  **Reinforcement Learning (RL):** Bots learn to perform core combat tasks (detection, aiming, firing) using Unity ML Agents.
2.  **Decentralized Communication:** Real-time battlefield data (enemy sightings, bot status) is shared across a simulated blockchain network, exemplified by the **ZetaChain** protocol's cross-chain capabilities.
3.  **Symbolic Reasoning:** Bots interpret complex, high-level commands and generate intelligent responses using the **MeTTa** (Meta-Type Theoretical Framework) language, allowing for flexible, non-rule-based behavior.

This project serves as a lightweight, open-source demonstration of decentralized AI agent capabilities for complex security or defense simulations.

---

## ✨ Key Features

| Feature | Technology | Description |
| :--- | :--- | :--- |
| **Swarm Learning** | Unity ML Agents (PPO) | Bots are trained to autonomously detect, track, and engage targets with high precision. |
| **Decentralized Data Sharing** | Simulated ZetaChain/Smart Contracts | Real-time intel (enemy positions, environmental data) is logged and shared among the swarm via smart contract interactions. |
| **Intelligent Scouting** | Dedicated Drone Agent | A non-combat drone scout provides initial and continuous intelligence (e.g., enemy heat signatures) to the swarm. |
| **Commander Interface** | Web UI (React/Next.js) | A human operator can issue high-level symbolic commands to the swarm. |
| **Symbolic Reasoning** | MeTTa (via Hyperon) | Bots process complex commands and environmental data using symbolic logic, enabling intelligent decision-making beyond simple rule trees. |

---

## 🛠️ Technology Stack

* **Simulation Engine:** Unity 2022.x+
* **AI Training:** Unity ML Agents (Reinforcement Learning)
* **Decentralized Network:** Simulated ZetaChain/EVM Smart Contracts (Solidity)
* **AI Reasoning:** MeTTa (Meta-Type Theoretical Framework)
* **Frontend/Commander UI:** React/Next.js (for web interface)
* **Networking:** WebSockets for communication between Unity and the Web3 layer.

---

## 🚀 Getting Started

### 1. Prerequisites

* Unity Editor (2022.x or newer)
* Python 3.8+ (for ML Agents and MeTTa server)
* Node.js and npm (for Commander Web UI)

### 2. Installation

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/YourUsername/project-chimera.git](https://github.com/YourUsername/project-chimera.git)
    cd project-chimera
    ```

2.  **Unity Setup:**
    * Open the `Unity/ProjectChimera` folder in the Unity Editor.
    * Ensure the ML Agents package is installed via the Package Manager.

3.  **Python Environment (RL & MeTTa):**
    ```bash
    # Create a virtual environment
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    
    # Install ML Agents, Hyperon (for MeTTa), and Web3 libraries
    pip install -r requirements.txt 
    ```

4.  **Web UI Setup (Commander):**
    ```bash
    cd commander-ui
    npm install
    # Note: Requires local smart contract deployment for full functionality (see Deployment).
    ```

### 3. Running the Simulation

1.  **Start the MeTTa/AI Reasoning Server:**
    * In the Python environment: `python me_server.py`

2.  **Start the Blockchain Listener/Data Relay:**
    * In a separate terminal: `python web3_relay.py` (simulates monitoring ZetaChain smart contract events).

3.  **Start the Commander Web UI:**
    * In the `commander-ui` directory: `npm run dev`
    * Open your browser to `http://localhost:3000`.

4.  **Run Unity:**
    * In the Unity Editor, open the `Scenes/MainSimulation` scene.
    * Press the **Play** button.

---

## 📚 Documentation & Architecture

* **`/Docs/`**: Contains detailed architectural diagrams, including the data flow between Unity, the Web3 layer, and the MeTTa reasoning engine.
* **`/Unity/Scripts/`**: Bot logic, RL agent implementation, and network handlers.
* **`/SmartContracts/`**: Solidity code for the simulated `IntelRegistry.sol` contract.
* **`/MeTTa/`**: Contains the symbolic reasoning knowledge base and MeTTa scripts (e.g., `command_parser.metta`).

## 🤝 Contributing

We welcome contributions from the community! Whether you are interested in:

* Improving the RL training efficiency.
* Expanding the MeTTa knowledge base for more complex reasoning.
* Integrating with a live testnet (e.g., ZetaChain testnet) instead of the simulated Web3 layer.
* Enhancing the Commander UI/UX.

Please refer to the `CONTRIBUTING.md` file for guidelines.

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

**Project Lead:** \[Daniel Githinji/Danterub.inc]

**Contact:** danterub@proton.me

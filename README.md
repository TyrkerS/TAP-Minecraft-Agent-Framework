# MINECRAFT AGENT FRAMEWORK

[![codecov](https://codecov.io/github/TyrkerS/Axies/graph/badge.svg?token=I1GK59EB31)](https://codecov.io/github/TyrkerS/Axies)

## ⭐ Project Summary
This project implements a **Python-based framework** for creating, controlling, and testing autonomous agents inside **Minecraft**.  
It provides a full environment for running behaviours, interacting with a Minecraft server, logging actions, and developing custom AI agents using Python.

The framework includes a ready‑to‑run Minecraft server, example agent code, and a modular architecture to define actions, goals, and behaviours. It was originally built for educational and experimentation purposes in game AI.

---

## 🧩 Technologies & Skills Demonstrated

### **Artificial Intelligence / Agent Systems**
- Behaviour-driven agents  
- Perception–action loop  
- Autonomous decision-making  
- State-based and rule-based behaviours  

### **Python Development**
- Modular code architecture  
- Class-based agent design  
- Logging, debugging and event callbacks  
- Testing environment with `pytest`  
- Clear project packaging and script handling  

### **Minecraft Integration**
- Communication between Python and a Minecraft server  
- Execution of agent actions in real time  
- Server automation through scripts (`StartServer.bat`)  

---

## 📁 Project Structure
```
AdventuresInMinecraft/
│
├── MyAdventures/                  → Python source code for agents and behaviours
│   ├── agent.py                   → Base agent class
│   ├── behaviours.py              → Behaviour definitions
│   ├── world.py                   → World interaction utilities
│   └── ...
│
├── Server/                        → Ready-to-run Minecraft server
│
├── StartServer.bat                → Script to launch the server on Windows
│
├── requirements.txt               → Python dependencies
├── pytest.ini                     → Testing configuration
├── .coveragerc / .coverage        → Coverage settings and output
└── README.md                      → Original project documentation
```

### Design Philosophy
- **Modular:** All agent components are separated into behaviours, actions, and world logic.  
- **Educational:** Built to teach agent design inside a real game engine.  
- **Extendable:** You can easily create your own agent by subclassing the base classes.  
- **Reproducible:** Includes full server, configs, and tests to run experiments consistently.

---

## 🔍 Project Details

### **1. Agent Logic**
Agents follow a classical AI loop:
1. Observe the Minecraft world  
2. Decide what action to perform  
3. Execute the action in the environment  
4. Log the behaviour

Built‑in tools allow agents to:
- move
- mine blocks
- interact with world objects
- follow scripted or autonomous goals

---

### **2. Behaviour System**
Behaviours are defined in `behaviours.py` and can include:
- wandering  
- item gathering  
- survival behaviours  
- goal-oriented actions  

The system is fully extensible.

---

### **3. World Interaction**
`world.py` provides high‑level functions to:
- detect entities  
- read blocks  
- modify or query the environment  
- send commands to the Minecraft server  

The agent does not interact directly with the server — instead it uses an abstraction layer for safety and clarity.

---

### **4. Testing**
The project includes:
- `pytest` test suite  
- coverage configuration  
- testable agent behaviours  

This ensures agents can be validated automatically.

---

## ▶️ How to Run the Project

### **1. Install dependencies**
```
pip install -r requirements.txt
```

### **2. Start the Minecraft server**
On Windows:
```
StartServer.bat
```

Alternatively, run the server inside the `Server/` directory manually.

### **3. Run the Python agent framework**
Inside `MyAdventures/`, run your agent:
```
python my_agent_script.py
```

Example agents can be found inside the same directory.

### **4. Run tests**
```
pytest
```

---

## ✔ Summary
This project provides a complete **Python AI agent framework for Minecraft**, including a dedicated server, behaviour system, and tools for world interaction.  
It demonstrates concepts in agent-based AI, Python architecture, and applied simulation inside a videogame environment — ideal for experimentation, teaching, or extending with custom behaviours.


# 🐍 AI Snake Game: Q-Learning Agent  
  
## 📌 Project Overview
An autonomous AI agent trained to play the classic Snake game using **Reinforcement Learning (Q-Learning)**. Instead of hardcoded rules, the agent learns optimal strategies through trial, error, and a reward-based system, successfully balancing exploration (random moves) and exploitation (using trained knowledge).

This project demonstrates foundational skills in building custom AI environments, applying mathematical decision-making algorithms, and tracking data metrics over time.

## 🚀 Key Features
*   **Custom Environment:** A lightweight, high-performance game grid built entirely from scratch using `pygame-ce`.
*   **Algorithmic Brain:** Implements a Q-Learning table/neural network to evaluate states and predict the most valuable next actions.
*   **Automated Data Logging:** Tracks epoch progression, maximum scores, and epsilon decay rates, automatically exporting training data to an Excel file using `pandas`.

## 🛠️ Tech Stack
*   **Language:** Python 3.12
*   **Environment & Rendering:** Pygame-CE (Community Edition)
*   **Math & Data Structures:** NumPy
*   **Data Logging:** Pandas, OpenPyXL

## 🧠 How the AI Learns (The 80/20 Breakdown)
The agent makes decisions based on a continuous loop of three factors:
1.  **State (Vision):** The AI observes its immediate surroundings (e.g., Is there a wall ahead? Is the food to the left?).
2.  **Action (Decision):** Based on the state, the AI chooses to move straight, turn left, or turn right.
3.  **Reward (Feedback):** The AI receives a positive reward (+10) for eating an apple and a negative penalty (-10) for crashing, adjusting its future decisions accordingly.

## ⚙️ Installation & Setup
Follow these steps to run the training environment on your local machine.

**1. Clone the repository**
```bash
git clone [https://github.com/YourUsername/Snake-Game-Q-Learning.git](https://github.com/YourUsername/Snake-Game-Q-Learning.git)
cd Snake-Game-Q-Learning


2. Create and activate a virtual environment

Bash
python -m venv myvenv
# On Windows:
myvenv\Scripts\activate
# On Mac/Linux:
source myvenv/bin/activate
3. Install dependencies

Bash
pip install -r requirements.txt
4. Run the Agent

Bash
python app.py
📁 Project Structure
app.py - The main game loop and visual environment rendering.

agent.py (or model.py) - The Q-Learning algorithm and decision-making logic.

requirements.txt - Project dependencies.

.gitignore - Excludes heavy virtual environment files and continuous Excel logs from version control.

👨‍💻 Developed by: Huzaifa Ansari 
Agentic AI Engineer.

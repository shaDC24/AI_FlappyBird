# 🐦 Flappy Bird AI with NEAT

This project is an implementation of the classic Flappy Bird game with an AI agent trained using [NEAT (NeuroEvolution of Augmenting Topologies)](https://neat-python.readthedocs.io/en/latest/). The game is built using the `pygame` library, and the AI learns to play the game by evolving neural networks.

---

## 📸 Demo

![Demo](demo.gif) <!-- Add a gif or image if available -->

---

## 🧠 How It Works

- The AI controls multiple birds using neural networks.
- Each bird is evaluated based on how far it goes without hitting pipes or the ground.
- NEAT evolves the neural networks across generations to improve performance.
- The network receives three inputs:
  1. Bird's current `y` position
  2. Distance to the top pipe
  3. Distance to the bottom pipe
- The network outputs a value:
  - If the output > 0.5, the bird jumps.

---

## 📦 Requirements

- Python 3.6+
- Pygame
- NEAT-Python

Install dependencies using pip:

```bash
pip install pygame neat-python


**📁 Project Structure**


flappy-bird-ai/
├── imgs/
│   ├── bird1.png
│   ├── bird2.png
│   ├── bird3.png
│   ├── pipe.png
│   ├── base.png
│   └── bg.png
├── config_feedforward_68c3f3d4a7.txt
├── main.py
└── README.md

**🛠️ Configuration**
The file config_feedforward_68c3f3d4a7.txt contains the NEAT settings (population size, network structure, mutation rates, etc.).

[NEAT]
fitness_criterion = max
fitness_threshold = 50
pop_size = 50
reset_on_extinction = False

[DefaultGenome]
...

**🚀 Running the Project**

python main.py


**🧬 NEAT Features**

Feedforward neural network
Speciation and fitness sharing
Dynamic topology evolution
Built-in reporting and statistics


This is a flappy bird game which is played by AI.I have learned this from  Tech with Tim.https://www.youtube.com/playlist?list=PLzMcBGfZo4-lwGZWXz5Qgta_YNX3_vLS2

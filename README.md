# 🐦 Flappy Bird AI with NEAT and Pygame

This project implements an AI that learns to play Flappy Bird using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. The AI controls birds that try to survive as long as possible, learning through evolution to jump over pipes.

## 📄 Features

- **Pygame-based Flappy Bird game**: Complete game logic, graphics, and animation.
- **NEAT algorithm integration**: The AI learns to play by evolving neural networks across generations.
- Multiple birds train simultaneously in each generation.
- Dynamic scoring and fitness calculation.

## 🧠 How it works

- Each bird has a neural network that decides when to jump.
- Birds receive inputs like their y-position and distances to pipes.
- NEAT evolves these networks to improve performance generation after generation.
- Fitness increases as birds survive longer and pass pipes.

## 🏗️ Project Structure
project/
├── imgs/
│ ├── bird1.png
│ ├── bird2.png
│ ├── bird3.png
│ ├── pipe.png
│ ├── base.png
│ └── bg.png
├── config-feedforward.txt
├── main.py
└── README.md

## 🖼️ Assets

Place the following images in an `imgs` folder:

- `bird1.png`, `bird2.png`, `bird3.png`: Bird animation frames
- `pipe.png`: Pipe image
- `base.png`: Ground/base image
- `bg.png`: Background image

## ⚙️ Requirements

- Python 3.x
- [pygame](https://www.pygame.org/news)
- [neat-python](https://github.com/CodeReclaimers/neat-python)

Install dependencies:

pip install pygame neat-python

▶️ Running the project

bash

python main.py

Make sure the config-feedforward.txt file is in the same directory. The NEAT configuration file controls parameters like population size, mutation rate, etc.

📝 NEAT Configuration
The config-feedforward.txt file defines settings for NEAT. You can adjust these to experiment with different evolution strategies and improve performance.

💡 Inspiration
This project is inspired by the idea of evolving neural networks to solve games and classic Flappy Bird clones. NEAT is a powerful evolutionary algorithm often used for these tasks.

🙌 Credits
NEAT algorithm by Kenneth O. Stanley

neat-python library

Pygame community for graphics and event handling

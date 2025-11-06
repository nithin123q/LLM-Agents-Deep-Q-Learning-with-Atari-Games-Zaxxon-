# LLM-Agents-Deep-Q-Learning-with-Atari-Games-Zaxxon-

readme_text = """
# 🕹️ Deep Q-Learning for Atari Games: **Zaxxon Agent Implementation**

**Author:** Nithin Yash Menezes  
**Course:** INFO 7375 – LLM Agents & Deep Q-Learning  
**Institution:** Northeastern University  
**Platform:** Google Colab  
**Notebook:** [Zaxxon.ipynb](https://colab.research.google.com/drive/1tJzHp9MaNftm4W9pUPZyHN1GwRXPZnqR#scrollTo=J7mLvANtTmrN)

---

## 🎯 Project Overview

This project implements a **Deep Q-Network (DQN)** agent to play the Atari game **Zaxxon** using the **Gymnasium Atari** environment (`ALE/Zaxxon-v5`).  
The goal is to train an RL agent that learns to maximize cumulative rewards by piloting a spaceship, avoiding obstacles, and shooting enemies.

The notebook follows a **modular, research-aligned design**, using **PyTorch**, **Gymnasium**, **ALE-py**, and **AutoROM** for seamless integration and visualization.

---

## ⚙️ Key Features

- ✅ **End-to-end RL pipeline**: from environment setup to recording gameplay.  
- 🧠 **Deep Q-Network (CNN-based)**: processes image frames into Q-values for each possible action.  
- 🔁 **Experience Replay**: samples past experiences to stabilize learning.  
- 🎯 **Epsilon-Greedy Policy**: balances exploration and exploitation.  
- 💾 **Model Checkpointing**: saves trained weights to `dqn_zaxxon.pt`.  
- 📹 **Video Recording**: records gameplay episodes using `RecordVideo`.  
- 🧩 **Evaluation Metrics**: average return and step count per episode.  
- ⚡ **Double DQN (Enhanced Trainer)**: reduces Q-value overestimation for better stability.

---

## 🧩 Environment Setup

The notebook installs and configures:
```bash
!pip install "gymnasium[atari,accept-rom-license]" "ale-py" "autorom[accept-rom-license]" opencv-python moviepy tqdm
!AutoROM --accept-license

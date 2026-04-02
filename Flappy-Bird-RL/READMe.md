# 🐦 Flappy Bird AI using Deep Q-Network (DQN)

## 📌 Overview

This project implements a **Reinforcement Learning agent** that learns to play Flappy Bird using a **Deep Q-Network (DQN)**.

The agent interacts with the environment, learns from rewards, and improves its performance over time to maximize survival.

---

## 🚀 Features

* Deep Q-Network (DQN) implementation
* Experience Replay for stable learning
* Target Network to reduce instability
* Epsilon-Greedy strategy for exploration vs exploitation
* Trained on Flappy Bird Gym environment

---

## 🧠 Tech Stack

* Python 🐍
* PyTorch 🔥
* Gymnasium 🎮
* NumPy

---

## 📂 Project Structure

```
├── bird.py                # Main file (training + testing)
├── dqn.py                 # Neural network architecture
├── experiencereplay.py    # Replay buffer implementation
├── parameters.yaml        # Hyperparameters
├── runs/                  # Logs & trained model (ignored)
└── README.md              # Project documentation
```

---

## ⚙️ Installation

### 1. Clone the repository

```
git clone https://github.com/vanshika64/Flappy-Bird-RL-DQN

```

### 2. Install dependencies

```
pip install torch gymnasium flappy-bird-gymnasium pyyaml
```

---

## 🏋️ Training the Model

Run the following command:

```
python bird.py default --train
```

👉 This will:

* Train the agent
* Save the model in `runs/`
* Log best rewards

---

## 🎮 Testing the Model

```
python bird.py default
```

👉 This will:

* Load trained model
* Run the game visually
* Agent plays automatically

---

## 📈 How It Works

1. Agent observes the environment (state)
2. Chooses action using epsilon-greedy policy
3. Stores experience in replay memory
4. Samples mini-batches to train neural network
5. Updates Q-values using Bellman equation
6. Synchronizes target network periodically

---

## 📊 Results

* Agent improves over time
* Learns to survive longer
* Maximizes cumulative reward

---

## ⚠️ Limitations

* Sensitive to hyperparameters
* Training can be slow
* May not generalize perfectly

---

## 🚀 Future Improvements

* Double DQN
* Dueling DQN
* Prioritized Experience Replay
* Hyperparameter tuning

---

## 💬 Conclusion

This project demonstrates how Deep Reinforcement Learning can be applied to solve sequential decision-making problems. The DQN agent successfully learns to play Flappy Bird by maximizing rewards through continuous interaction with the environment.

-
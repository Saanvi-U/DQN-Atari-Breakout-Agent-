# 🎮 DQN Atari Breakout Agent with Autoencoder Visualization

This project demonstrates a Deep Q-Network (DQN) agent trained to play the Atari Breakout game using deep reinforcement learning, enhanced with visualizations and an autoencoder-based state reconstruction system.

---

## 📌 Project Overview

- Train a DQN agent to play Breakout using convolutional neural networks.
- Monitor training via:
  - Reward plots
  - Epsilon decay visualization
  - Loss curves
- Autoencoder is used to compress and reconstruct game frames to analyze state representations learned.

---

## 🧠 Model Architecture

### 🔹 DQN (Deep Q-Network)
- Input: `(84, 84)` grayscale frame
- CNN Layers:
  - `Conv2D(32, 8x8, stride 4)`
  - `Conv2D(64, 4x4, stride 2)`
  - `Conv2D(64, 3x3, stride 1)`
- Dense Layers:
  - `Dense(512)`
  - `Dense(num_actions)` for Q-values

### 🔄 Autoencoder
Used to reconstruct input frames:
- Encoder: 2 Conv + MaxPooling layers
- Decoder: 2 Conv + UpSampling layers

---

## 📊 Visualizations

✅ **Reward per Episode**  
📉 **Loss Curve**  
🔀 **Epsilon Decay Over Time**  
📈 **Moving Average Reward**  
🖼️ **Original vs Reconstructed State Images**

---



## 🔪 Dependencies

```
tensorflow
keras
matplotlib
numpy
opencv-python
gym[atari]
```


---

## 📊 Metrics & Results

- ✅ Agent trained over 100 episodes with epsilon-greedy strategy
- 🔀 Target network updated every 10 episodes
- 🎯 Final reward trends show improved policy over time
- 🎨 Autoencoder learns a reasonable compression of input frames

---



## 📄 Google Colab Link

https://colab.research.google.com/drive/1ZD7rF-s7EfPTPeDjUDjPrmKScjxLbDNM?usp=sharing 




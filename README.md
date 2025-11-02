# 🎮 Super Mario Bros Reinforcement Learning

[![Python](https://img.shields.io/badge/python-3.13%2B-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Stable-Baselines3](https://img.shields.io/badge/Stable%20Baselines3-2.7.0-blue.svg)](https://stable-baselines3.readthedocs.io/)
[![Gymnasium](https://img.shields.io/badge/Gymnasium-1.2.1-brightgreen.svg)](https://gymnasium.farama.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/tooichitake/gymnasium-mario?style=social)](https://github.com/tooichitake/gymnasium-mario/stargazers)

> 🚀 **Train AI agents to play Super Mario Bros using deep reinforcement learning with A2C**

## 🎬 Trained Agent Demo

Watch our A2C agent playing Super Mario Bros after training:

https://github.com/user-attachments/assets/06de1fdb-ad08-413f-8118-d5286a815a6c

*Agent trained with CNN-based observations (video appears 4x speed due to frame_skip=4)*

## 🌟 Key Features

- **IMPALA CNN Architecture**: ResNet-style visual feature extraction
- **Environment Wrappers**: Random noop reset, maxpooling and frame Skip, grayscale Frame Warp, frame stack 
- **Hyperparameter Tuning**: Distributed optimization with automatic checkpoint recovery
- **Training Scripts**: Simple train/test/continue workflow
- **Monitoring**: TensorBoard logging and video recording

## 🛠️ Installation

### Prerequisites

- Python 3.10 or higher (3.13+ recommended for better performance)
- C++ compiler (for NES emulator)
- Conda (recommended)

### Quick Install

#### Windows

```bash
# Clone the repository
git clone https://github.com/SiddiqurRahman3802/gymnasium-mario-a2c.git
cd gymnasium-mario

# Create conda environment
conda create -n mario python=3.13 -y
conda activate mario

# Install all dependencies
pip install .
```

#### Linux / AWS SageMaker

**First-time setup** (run once):
```bash
# Initialize conda for bash
conda init bash

# Restart shell to apply changes
exec bash
```

**Then install the project**:
```bash
# Clone the repository
git clone https://github.com/SiddiqurRahman3802/gymnasium-mario-a2c.git
cd gymnasium-mario

# Create and activate conda environment
conda create -n mario python=3.13 -y
conda activate mario

# Install all dependencies
pip install .
```

### Training Output Structure

```
results/
├── a2c/
│   └── exp7/
│       ├── models/           # Model checkpoints
│       ├── logs/             # TensorBoard logs
│       └── videos/           # Gameplay recordings
└── a2c_tuning_v4/
    └── a2c/
        ├── best_params_v4.json          
        ├── optuna_a2c_v4.sqlite4
        └── optuna_trials_v4.csv
```

## 👏 Credits

### Authors
- **Md Siddiqur Rahman**


## 📄 License

MIT License - see LICENSE file for details

---

<p align="center">
  Made with ❤️ for the RL community
</p>

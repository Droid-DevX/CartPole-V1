# Reinforcement Learning – CartPole with Stable-Baselines3

A reinforcement learning project for training agents to solve the classic CartPole-v1 control problem using policy-based and value-based algorithms.

## Description

This project implements an end-to-end reinforcement learning pipeline for training and evaluating agents on the CartPole-v1 environment. It applies PPO and DQN algorithms using Stable-Baselines3, with vectorized environments for efficient training and TensorBoard for real-time learning visualization. The system includes model saving and reloading for reproducibility, early stopping via reward threshold callbacks, and custom policy and value network architectures. Quantitative evaluation is performed using mean episode rewards, and algorithm comparison between PPO and DQN is included to benchmark performance.

## Getting Started

### Dependencies

* Python 3.x
* Required libraries listed in `requirements.txt` (including Stable-Baselines3, Gymnasium, PyTorch, TensorBoard)
* Compatible with Windows, macOS, and Linux

### Installing

1. Download or clone the repository:

```
git clone https://github.com/Droid-DevX/CartPole-V1

```

2. Install required dependencies:

```
pip install -r requirements.txt
```

3. Ensure the following files are present after training:
   * `ppo_cartpole.zip` – saved PPO model
   * `dqn_cartpole.zip` – saved DQN model

### Executing program

1. Train the PPO agent:

```
python train_ppo.py
```

2. Train and compare with DQN:

```
python train_dqn.py
```

3. Evaluate a saved model:

```
python evaluate.py
```

4. Launch TensorBoard to monitor training:

```
tensorboard --logdir ./logs
```

## Help

Common issues:

* Missing model files: Run the training script first to generate `.zip` model files.
* Module import errors: Reinstall dependencies:

```
pip install -r requirements.txt
```

* TensorBoard not updating: Ensure the `--logdir` path matches the logging directory used during training.

## Authors

Contributors names and contact info

* Your Name
   * GitHub: (https://github.com/Droid-DevX)

## Version History

* 0.2
   * Algorithm comparison: PPO vs DQN added
   * Early stopping callbacks implemented
   * Custom policy and value network architectures
   * TensorBoard logging integrated
* 0.1
   * Initial PPO agent with basic vectorized environment setup

## License

This project is licensed under the MIT License. See the `LICENSE` file for full details.

## Acknowledgments

Inspiration, code snippets, and references:

* OpenAI Gymnasium (CartPole-v1 environment)
* Stable-Baselines3
* PyTorch
* TensorBoard
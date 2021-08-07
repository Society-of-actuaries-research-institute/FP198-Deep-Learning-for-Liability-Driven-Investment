# LDI_DL
Deep Learning for Liability Driven Investment

This program is a reinforcement learning example to solve a simplified DB pension plan dynamic LDI strategy optimization. It is part of the research project "Deep Learning for LDI" sponsored by the Society of Actuaries. The program is intended for educational purpose.

It is coded in Python using PyTorch, which is an open source deep learning package.

The sample program is saved as an Jupyter Notebook has been tested using Python3.7. It is runnable on either CPUs or GPUs

# File Structure 
**Root folder**

RL_Script_Sample.ipynb: The main script in Jupyter Notebook which is self explained. It contains ESG, asset and liability projection, model setup and model training. It uses reinforcement learning with deep learning models (fully connected neural networks and long short term memory models) to approximate the reward function. It solves a simple question: what investment strategy is appropriate given economic conditions and funding status. It has four models:

RL1: LSTM model with rebalance constraints

RL2: LSTM model without rebalance constraints

RL3: FCNN model with rebalance constraints

RL4: FCNN model without rebalance constraints

The script is for illustration purpose which means for practical usage, parallel computing needed to be included as the dynamic projection is an expensive task. Model hyperparameters are also set so that the program can be finished in a few minutes. However, for real model convergence, a lot more iterations are needed.

**Subfolder**

input: Files containing model assumptions, pregenearted scenarios (test_states.zip) and plan status dynamic projection (liab.csv).

test_states.zip needs to be unzipped so that the script can make reference to the file in csv format.

# Run Program
1. To run model, open the notebook with Jupyter Notebook and conduct the run.
2. The notebook can also be saved as a py file test.py and can be run using "python test.py"

# IHC_attidute_control

## Abstract

This project aim to develop a neural network estimate control parameter or direcly control a specific feature of a designed object learning its dynamic.

## Enviroment
I designed a control schema in Simulink in a way to verify system and its performance. Python'r API have been used.

## Methodology
The development of the the code follows these key steps:

1. **Study of the dynamic system**: Tested several control schemas in order to understand the dynamic of the object and understand how to control it.

2. **TCP/ICP communication**: Communication Simulink-Python with a TCP/ICP connection to collect data such as the desired trajectory, reference model output, controlled object position and error.

3. **Model Architecture**: Feed forward network is used for estimate PID parameters [1] and Actor-Critc architecture for reinforcement learning approach [2].

4. **Training**: Feed forward network data have been trained by collecting information in a dataset and training on it. For the Actor-Critic architecture I used information from Simulink in order to estimate the state with Critic network and choose a control action with Actor network.


## Usage

To utilize the "Geometric Transformers" project, follow these steps:

1. **Install Dependencies**: 
    - Ensure all required dependencies are installed. 
    - Matlab engine can be installed following the documentation avaible on matlab's website (https://it.mathworks.com/help/matlab/matlab_external/install-the-matlab-engine-for-python.html). 
    - If doesn't work, you still need one more passage. Create an environment variable PYTHONPATH with value 'path_to_setupd.py'.

2. **Set hyperparameters**: Set hyperparameters in the code in order to automatize everything


## References
[1] An Attitude Control Method of Aircraft Based on Neural Network Batch Training Strategy (https://ieeexplore.ieee.org/document/9327655)

[2] (https://www.mdpi.com/2313-7673/8/5/434)


